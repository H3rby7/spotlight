# **Ultra-wideband (UWB)**

UWB is a short-distance RF technology. 

* Precision < 30cm
* Ability to detect height changes
* Up to 100 position updates per second
* Few interferences
* Higher costs 

[Source](https://www.industry-of-things.de/indoor-positionsbestimmung-ortungstechniken-im-vergleich-a-632311/) (in german)

# ** Bluetooth 5.1 **

* Bluetooth 5.1 by specification can detect the Angle of Arrival (AoA)
[Source](https://www.industry-of-things.de/bluetooth-51-richtungserkennung-mit-angle-of-arrival-a-919815/) (in german)
* [Raspberry Pi 4 does not have BTLE 5.1](https://www.raspberrypi.org/forums/viewtopic.php?t=257718)

## Nordic Semiconductor Chips

https://www.nordicsemi.com/Products/Low-power-short-range-wireless/Direction-finding

These nordic chips have the technical power for Bluetooth LE 5.1 AoA. The are a SOC (system on a chip)

Number | tested?
--- | --- 
5340 | nope
52833 | nope
52820 | nope
52811 | (ordered)

Attention: These chips as of now do not have a development KIT available and by themselves are very tiny,
which made them impossible for me to connect.

# WIFI scanning

https://github.com/schollz/find-lf

Disadvantage - old outdated repo. Defines position, we would need the light position as well and calculate the angle.

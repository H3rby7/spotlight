# Autospot

Idea is to have a "Moving-Head" (a light) connected to a form of beacon. The light will always point to that beacon.

## Further

It may be possible to control more feature of the Moving-Head with an app or voice commands or gestures or whatever really

* I heard there is also a form of bluetooth ring that might do the trick.

# Technology

I researched a couple of possible technologies. Many of them are used in industry for highly automated production environments for position/location/direction finding.

TLDR: My first try will be [bluetooth 5.1 with "Angle of Arrival (AoA)"](https://www.bluetooth.com/blog/new-aoa-aod-bluetooth-capabilities/) 
with the [nRF52811 chip](https://www.nordicsemi.com/Products/Low-power-short-range-wireless/nRF52811/GetStarted).
I do not work for nordic or anything ;)


See [Technology](./research/Technologies.md)

# Approach

## Next

- [x] Find documentation files
- [x] Setup next steps
- [ ] Wire nRF52811 to Arduino Board
    - [ ] [Hardware wiring](https://infocenter.nordicsemi.com/index.jsp?topic=%2Fug_nrf52840_dk%2FUG%2Fcommon%2Fnordic_tools.html)
        - [ ] Antenna Array (MAke sure to Follow PCB Guidelines as in nRF52811 spec, 7.3.8)
    - [ ] Check for bluetooth to work (How is to be determined)
- [ ] A beacon sending a constant signal, received by arduino
- [ ] Setup AoA mode for nRF52811 
- [ ] Receive IQ data (basically the raw data) and dump to CSV
- [ ] Visualize IQ data in excel or something
- [ ] Interpret Data / Use one of the AoA algorithms

Then get a movinghead and wire it up.
 
    
## Reads

- [ ] [Bluetooth 5.1 Core Specification Vol 6 Part B](./research/ext_resources/Core_v5.1.pdf)
- [ ] [nRF52811 Product Specification](./research/ext_resources/nRF52811_PS_v1.0.pdf)  chapter 6.14.12

# Setup

[Here are my steps so far](./research/Setup-Done.md)

### (hypothetical, right now I do not know what is necessary)

https://infocenter.nordicsemi.com/index.jsp?topic=%2Fug_nrf52840_dk%2FUG%2Fcommon%2Fnordic_tools.html

* GNU/GCC as we are programming C something
* 

# Useful Links

* https://devzone.nordicsemi.com/
* [Docs nRF52811](https://infocenter.nordicsemi.com/index.jsp?topic=%2Fstruct_nrf52%2Fstruct%2Fnrf52811.html&cp=3_3)
* [Docs DevKit for nRF52840](https://infocenter.nordicsemi.com/index.jsp?topic=%2Fug_nrf52840_dk%2FUG%2Fnrf52840_DK%2Fkit_content.html)
* [Some Q&A on 5.1 AoA with nRF52811](https://devzone.nordicsemi.com/f/nordic-q-a/53729/nrf52811-aoa-mode-config)
* [Nordic SOC DK](https://www.nordicsemi.com/Software-and-tools/Software/nRF5-SDK)
sadly only emulates the 52811, and does not support Direction Finding.
* [Arduino adoption of nordic SDK](https://github.com/sandeepmistry/arduino-nRF5)
* [Another Adruino LIB](https://github.com/adafruit/Adafruit_nRF52_Arduino) - probably faster to adopt BT5.1

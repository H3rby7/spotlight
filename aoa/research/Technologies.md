A breakdown of my research

# **Ultra-wideband (UWB)**

(in german for now, sorry - text has been copy pasted from somehwere)

Ultra-wideband ist eine Kurzstrecken-Funktechnik. Die Genauigkeit liegt bei unter 30 Zentimetern und ist damit deutlich höher als die von Beacons oder WLAN. Auch Höhenunterschiede können sehr genau ermittelt werden.

| **Vorteile**                                                 | **Schwächen**                                                | **geeignete Anwendung**                                      |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| hohe Genauigkeitniedrige Latenzzeiten (bis zu 100 Positionsupdates pro Sekunde)kaum Interferenzen | höhere Kosten und kürzere Batterielebensdauer als BLE Beacons | Tracking-Lösungen im industriellen Umfeld mit hoher Präzisionsanforderung und geringer Anzahl an Assets |

 Quelle: https://www.industry-of-things.de/indoor-positionsbestimmung-ortungstechniken-im-vergleich-a-632311/

Oder nur Richtung (ausreichend, da Licht ein Strahl ist) - UWB muss glaube ich position bestimmen

# ** Bluetooth 5.1 **

Bluetooth 5.1 hat eine Richtungserkennung

https://www.industry-of-things.de/bluetooth-51-richtungserkennung-mit-angle-of-arrival-a-919815/

(btw. Pi4b wird dsa nicht selbst können -> https://www.raspberrypi.org/forums/viewtopic.php?t=257718)

Nordic chips:

https://www.nordicsemi.com/Products/Low-power-short-range-wireless/Direction-finding

## Nordic Semiconductor Chips

These nordic chips have the technical power for Bluetooth LE 5.1 AoA. The are a SOC (system on a chip)

Number | tested?
--- | --- 
5340 | nope
52833 | nope
52820 | nope
52811 | (ordered)

# WIFI scanning

https://github.com/schollz/find-lf

Disadvantage - old outdated repo. Defines position, we would need the light position as well and calculate the angle.

# Setup done

This describes all steps as i made them for my first-time setup.
So some of this will be unnecessary, but necessary to keep track of all I did.

Check out the [things I tried, that did not work](tried-but-failed.md)

## Steps

1. Install and prepare you Arduino IDE 1.8.13 (Windows Store 1.8.42)
1. Add additional boards in Arduino IDE: https://sandeepmistry.github.io/arduino-nRF5/package_nRF5_boards_index.json
1. Install BLEPeripheral in Arduino IDE Libraries
1. Install [JLINK drivers/binaries](https://www.segger.com/downloads/jlink/) - I don't have a DK nor a JLINK device, so this can go again.
1. Uninstalled SEGGER JLINK
1. Download SoftDevice [113](https://www.nordicsemi.com/Software-and-tools/Software/S113/Download), but only 132 is available in IDE with sandeepmistry's lib)
1. Removed the boards from sandeepmsitry and the json url. 


Next: Try adafruit lib - I hope to get at least some board layouts done.

E.G.: the exact nRF chip is not present but I assume the chips are somewhat similarly wired and thus I can use these libs to do my wiring virtually.

1. Add additional boards in Arduino IDE: https://www.adafruit.com/package_adafruit_index.json
1. Install nRF boards

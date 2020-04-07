# NixieTubesShieldNCS314

## About
The firmware found in this repository is being written and modified to improve / tweak the functionality of a [GRA & AFCH](http://gra-afch.com) [NCS312 v1.3](https://gra-afch.com/catalog/nixie-tubes-clocks/nixie-tubes-clock-arduino-shield-ncs312-for-xussr-in-12-nixie-tubes/) Nixie tube shield connected to an Arduino Mega 2560.  The use of the shield and firmware allows the Arduino to become a full 6-digit IN-12 Nixie tube clock with neon dot digit separators (between the hours/minutes/seconds displays).

## Known Issues
1. **IRremote Library**
	- For reasons unknown, the most recent version of the IRremote library fails to compile for the Arduino Mega 2560 (and possibly other boards as well).  Until the problems are fixed, it is advised to use the version of the library found at [Libraries/IRremote](Libraries/IRremote).

## List of Changes
### Control booleans
1. [STARTUP_PLAY_TEST_SONG](https://github.com/ckuzma/NixieTubesShieldNCS314/blob/master/Firmware/NixieClockShield_NCS314/NixieClockShield_NCS314.ino#L75)
	- Enables or disables the (loud) test song on startup
2. [STARTUP_DO_LIGHT_SHOW](https://github.com/ckuzma/NixieTubesShieldNCS314/blob/master/Firmware/NixieClockShield_NCS314/NixieClockShield_NCS314.ino#L76)
	- Enables or disables the LED light show / test on startup
	- One color of LED flashes briefly still, but no effort was added to fix this
3. [FLASH_NEON_SEPARATORS](https://github.com/ckuzma/NixieTubesShieldNCS314/blob/master/Firmware/NixieClockShield_NCS314/NixieClockShield_NCS314.ino#L77)
	- Enables or disables the flashing of the neon neon digit separators
4. [SHOW_DATE_INTERMITTENTLY](https://github.com/ckuzma/NixieTubesShieldNCS314/blob/master/Firmware/NixieClockShield_NCS314/NixieClockShield_NCS314.ino#L78)
	- Enables or disables the display of the current date whenever the anti-poisoning routine runs

## Credit
This is a fork of the original [NixeTubesShieldNCS314](https://github.com/afch/NixeTubesShieldNCS314) project as written by [afch](https://github.com/afch).  That original project consisted a number of firmwares, both compiled and uncompiled, for loading onto various Arduino boards mated with Nixie tube clock shields made by [GRA & AFCH](http://gra-afch.com), who can also be contacted at [fominalec@gra-afch.com](mailto:fominalec@gra-afch.com).  For information on the shields themselves or answers as to why the firmware was written the way it is, please see [their website](http://gra-afch.com).


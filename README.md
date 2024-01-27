# NixieTubesShieldNCS314

## About
The firmware code found in this repository is a modified fork of pre-existing work in order to make it more user-friendly.  More specifically, modifiers were added (see "List of Changes" below) to enable/disable particular functionality with simple boolean flags.

This firmware was specifically compiled for the ["Hardware Version 2.x" version of the NCS312 v1.3](https://gra-afch.com/catalog/nixie-tubes-clocks/nixie-tubes-clock-arduino-shield-ncs312-for-xussr-in-12-nixie-tubes/) nixie tube clock shield running on an Arduino Mega 2560.  It should also be compatible with Arduino Uno-type boards, though GPS functionality will be lost.

## List of Changes
### Control booleans
1. [STARTUP_PLAY_TEST_SONG](https://github.com/ckuzma/NixieTubesShieldNCS314/blob/19ecd705d4d68c30db8a44c294fcc924ac78f0de/Firmware/Hardware%20Version%202.x%20(HW2.x)/NixieClockShield_NCS314/NixieClockShield_NCS314.ino#L89)
	- Enables or disables the (loud) test song on startup
2. [STARTUP_DO_LIGHT_SHOW](https://github.com/ckuzma/NixieTubesShieldNCS314/blob/19ecd705d4d68c30db8a44c294fcc924ac78f0de/Firmware/Hardware%20Version%202.x%20(HW2.x)/NixieClockShield_NCS314/NixieClockShield_NCS314.ino#L90)
	- Enables or disables the LED light show / test on startup
3. [FLASH_NEON_SEPARATORS](https://github.com/ckuzma/NixieTubesShieldNCS314/blob/19ecd705d4d68c30db8a44c294fcc924ac78f0de/Firmware/Hardware%20Version%202.x%20(HW2.x)/NixieClockShield_NCS314/NixieClockShield_NCS314.ino#L91)
	- Enables or disables the flashing of the neon digit separators
	- This was added so that I could quickly toggle on/off the neon digits on my clock as one of them failed and only blinking three looked tacky
4. [SHOW_DATE_INTERMITTENTLY](https://github.com/ckuzma/NixieTubesShieldNCS314/blob/19ecd705d4d68c30db8a44c294fcc924ac78f0de/Firmware/Hardware%20Version%202.x%20(HW2.x)/NixieClockShield_NCS314/NixieClockShield_NCS314.ino#L92)
	- Enables or disables the display of the current date whenever the anti-poisoning routine runs
5. [NIGHT_MODE_ENABLED](https://github.com/ckuzma/NixieTubesShieldNCS314/blob/19ecd705d4d68c30db8a44c294fcc924ac78f0de/Firmware/Hardware%20Version%202.x%20(HW2.x)/NixieClockShield_NCS314/NixieClockShield_NCS314.ino#L93)
	- Enables or disables the shutdown of the display at night, a feature that was added with v1.98

## Credit
This is a fork of the original [NixeTubesShieldNCS314](https://github.com/afch/NixeTubesShieldNCS314) project as written by [afch](https://github.com/afch).  That original project consisted a number of firmwares, both compiled and uncompiled, for loading onto various Arduino boards mated with Nixie tube clock shields made by [GRA & AFCH](http://gra-afch.com), who can also be contacted at [fominalec@gra-afch.com](mailto:fominalec@gra-afch.com).  For information on the shields themselves or answers as to why the firmware was written the way it is, please see [their website](http://gra-afch.com).


BlueBasic
=========

NOTE: I no longer have access to either hardware or tools to update the builds.

BASIC interpreter for CC2540 and CC2541 Bluetooth LE chips.

This project contains a BASIC interpreter which can be flashed onto a CC2540 or CC2541 Bluetooth module. Once installed, simple use the Bluetooth Console tool to connect and start coding on the device using good old BASIC.

The project was inspired by experimenting with the HM-10 modules (a cheap BLE module) and a need to provide an easy way to prototype ideas (rather than coding in C using the very expensive IAR compiler). Hopefully other will find this useful.

For more information see https://github.com/aanon4/BlueBasic/wiki/Blue-Basic:-An-Introduction


========== Build Instructions ==============

build process is slightly more involved due to OAD feature.

there are 3 packages to compile util, blueBasicLoader & blueBasic. 

blueBasic post build calls a script that creates the combined bin/hex files

so util and blueBasicLoader must be compiled 1st.

I used IAR 9.3 for all builds

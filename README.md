BlueBasic
=========

NOTE: I no longer have access to either hardware or tools to update the builds.

BASIC interpreter for CC2540 and CC2541 Bluetooth LE chips.

This project contains a BASIC interpreter which can be flashed onto a CC2540 or CC2541 Bluetooth module. Once installed, simple use the Bluetooth Console tool to connect and start coding on the device using good old BASIC.

The project was inspired by experimenting with the HM-10 modules (a cheap BLE module) and a need to provide an easy way to prototype ideas (rather than coding in C using the very expensive IAR compiler). Hopefully other will find this useful.

For more information see https://github.com/aanon4/BlueBasic/wiki/Blue-Basic:-An-Introduction

youyube video: https://www.youtube.com/watch?v=gd_tHgKUJbI

https://hackaday.io/project/2386-bluebasic-basic-for-bluetooth

https://github.com/aanon4/BlueBasic

For those interested, here is the Pin mapping for the HM-10 to Blue Basic commands: 

HM-10   HM-10         CC254X    Blue
Pin         IO Name    IO Name    Basic
23          PIO0          P1_3           P1(3)
24          PIO1           P1_2           P1(2)
25          PIO2          P1_1            P1(1)
26          PIO3          P1_0           P1(0)
27          PIO4          P0_7           P0(7)
28          PIO5          P0_6          P0(6)
29          PIO6          P0_5          P0(5)
30          PIO7          P0_4          P0(4)
31           PIO8          P0_3          P0(3)
32          PIO9          P0_2          P0(2)
33          PIOA          P0_1           P0(1)
34          PIOB          P0_0          P0(0)

Of course, this can be found deeper in Tim's blog which I have just discovered.



forked project botspine
updated basic wiki:
https://github.com/kaiateic/BotSpine/wiki



breakout boards:
https://oshpark.com/shared_projects/aWRbRvyh

https://oshpark.com/shared_projects/puBoiqUm



========== Build Instructions ==============

build process is slightly more involved due to OAD feature.

there are 3 packages to compile util, blueBasicLoader & blueBasic. 

blueBasic post build calls a script that creates the combined bin/hex files

so util and blueBasicLoader must be compiled 1st.

I used IAR 9.3 for all builds

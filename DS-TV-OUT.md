# Nintendo DS-TV-OUT Restoration Project

## Introduction

During late 2020, we discovered that the Nintendo DS Lite had a leftover feature in its SoC allowing it to easily have hardware video output. With a little circuitry and some software hacks, we were able to restore it and make it usable for anyone! No FPGA's, no bulky or cumbersome hardware.

## Software

The retail firmware of the Nintendo DS Lite (not the BIOS) disables this specific feature early in the boot process. To reenable it, we can just use a custom firmware like flashme, which is very easy to install and is required only once. Despite that, we are working on an even simpler solution to make it available to as many people as possible.

## Hardware

This feature is only found on the Nintendo DS Lite. Nintendo DS Phat does not contain this feature nor does the Nintendo DSi. It is important to remark that **this is not the same hardware** found on Devkits or other special units. This hardware feature is present in virtually **every single Nintendo DS Lite** out there. The reason why it was left there is unknown, but as said before, it is not related to development units, those use a different video capture hardware. Maybe Nintendo imagined the Nintendo Switch as early as 2006?

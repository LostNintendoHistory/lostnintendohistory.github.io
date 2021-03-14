# Nintendo DS-TV-OUT Restoration Project

## Introduction

During late 2020, we discovered that the Nintendo DS Lite had a leftover feature in its SoC allowing it to easily have cheap hardware video output. With a little circuitry and some software hacks, we were able to restore it and make it usable for anyone. No FPGA's, no bulky or cumbersome hardware. This mod is specially useful to revive consoles with only the lower screen, being able to watch the upper screen on your TV. Or to create a GBA Macro with additional TV Output.

<center>
<img src="https://raw.githubusercontent.com/LostNintendoHistory/lostnintendohistory.github.io/main/img/NDSTVOUT/DSTVOUT.jpg" width="250" height="250"><br></center>
<center>
  <b>First iteration of the TV-OUT board in action</b>
  </center>

## Installation Steps

If you are just interested in installation, this is the current method **while we work on simpler methods** and more features you have requested:

1. Follow [these steps](https://github.com/LostNintendoHistory/Lost-NDS-TV/tree/main/fwpatch) to install our Custom Firmware that enables the TV Output.
2. Plug the board into the upper screen socket
3. Enjoy your TV Output

## Installation Video Tutorial

[![NDS TV OUT Installation Tutorial by radioactivepeter](https://img.youtube.com/vi/lBJaaE3PBwQ/0.jpg)](https://www.youtube.com/watch?v=lBJaaE3PBwQ)

---

## Software

The retail firmware of the Nintendo DS Lite disables this specific feature early in the boot process. To reenable it, we use a custom firmware with patches, which is very easy to install. 

## Hardware

This feature is only found on the Nintendo DS Lite. Nintendo DS Phat does not contain this feature nor does the Nintendo DSi. It is important to remark that **this is not the same hardware** found on Devkits or other special units. This hardware feature is present in virtually **every single Nintendo DS Lite** out there. The reason why it was left there is unknown, but as said before, it is not related to development units, those use a different video capture hardware. Perhaps Nintendo imagined the Nintendo Switch as early as 2006?

<center><img src="https://raw.githubusercontent.com/LostNintendoHistory/lostnintendohistory.github.io/main/img/NDSTVOUT/PCB_Rev_11.png" width="350" height="400"></center>


We only need a few extra hardware components to make this video signal usable. You will be able to download the schematics and gerber files for our open hardware circuit board [from the repository](https://github.com/LostNintendoHistory/Lost-NDS-TV). The latest version is revision 1.2 which fixes some minor issues with a component in the board.

<center>
<img src="https://raw.githubusercontent.com/LostNintendoHistory/lostnintendohistory.github.io/main/img/NDSTVOUT/Prototype.jpg" width="350" height="350"><br>
</center>
<center>
  <b>First prototype and tests before designing a proper board</b></center><br>
  


The final, production-ready board contains a DAC (Digital to Analogue Converter) which turns the 10 bits digital signal at 16.7 MHz provided by the DS Lite into a proper analogue signal. This signal then goes through an operational amplifier and it's ready to be delivered to your nearest TV trough composite video.

We are currently considering creating an additional PCB revision which would allow to install the mod on consoles without lossing a working upper screen.



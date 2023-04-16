# Xbox Power LED RGB Circle Mod with Raspberry Pi Pico

This project demonstrates how to create a cycling RGB circle effect for the Original Xbox's power LED using a Raspberry Pi Pico and two WS2812 LEDs. The MicroPython script provided in this repository controls the LEDs and cycles them through the rainbow colors with a slight offset to create the desired effect.

⚠️ **WARNING:** Don't open up an Xbox if you don't know what you're doing, as the PSU internals are exposed and can still hold high voltages for a long time, making it dangerous. I take no responsibility for any damage to an Xbox if you do choose to open one up. ⚠️

It should also be noted, as you will see in my Hackster/Electromaker pages below, that I had issues with this project as trying to fit a microcontroller into an Xbox is rather tricky.
Make sure to check the pages out for more info on the project and how I actually came up with a better solution; I put the code here because it's handy to have.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Hardware Setup](#hardware-setup)
- [Software Setup](#software-setup)
- [References](#references)

## Prerequisites
- Original Xbox Console
- Raspberry Pi Pico
- 2x WS2812 RGB LEDs
- Protoboard and jumper wires
- Soldering iron and solder
- Hot glue gun
- Micro-USB cable for the Raspberry Pi Pico

## Hardware Setup
For a detailed guide on connecting WS2812 LEDs to a Raspberry Pi Pico, check out this tutorial: [How to control a NeoPixel LED strip with a Raspberry Pi Pico](https://www.freva.com/how-to-control-a-neopixel-led-strip-with-a-raspberry-pi-pico/)

Additionally, here is the hardware setup and config for the Xbox:

[Hackster.io](https://www.hackster.io/314reactor/xbox-rgb-led-2-0-528993)
[Electromaker.io](https://www.electromaker.io/profile/314Reactor)

## Software Setup
1. Connect the Raspberry Pi Pico to your computer using the Micro-USB cable.
2. Install MicroPython on the Pico following the instructions [here](https://www.raspberrypi.com/documentation/microcontrollers/micropython.html)
3. Change the PIN_NUM var in the `main.py` script to match the pin you connected the WS2812 LEDs to.
4. Upload the `main.py` script from this repository to the Raspberry Pi Pico using Thonny, more info [here](https://projects.raspberrypi.org/en/projects/getting-started-with-the-pico/5).

## Usage
1. Power on the Raspberry Pi Pico by connecting it to a USB power source.
2. The two WS2812 LEDs should now cycle through the rainbow colors with a slight offset between them.

## References
- [How to control a NeoPixel LED strip with a Raspberry Pi Pico](https://www.freva.com/how-to-control-a-neopixel-led-strip-with-a-raspberry-pi-pico/)
- [Raspberry Pi Pico MicroPython](https://www.raspberrypi.com/documentation/microcontrollers/micropython.html)
- [Getting Started with the Raspberry Pi Pico & Thonny](https://projects.raspberrypi.org/en/projects/getting-started-with-the-pico/5)
- [Hackster.io project link](https://www.hackster.io/314reactor/xbox-rgb-led-2-0-528993)
- [Electromaker.io project link](https://www.electromaker.io/profile/314Reactor)

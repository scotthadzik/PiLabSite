---
layout: default
title: Introduction to the Raspberry Pi
nav_order: 1
---
<p align="center">
<iframe width="560" height="315" src="https://www.youtube.com/embed/frOM7ITbsGg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

</p>

# 1. Raspberry Pi - A Single Board Computer

The [Raspberry Pi 4](https://www.raspberrypi.com/products/raspberry-pi-4-model-b/)
is a credit card size computer that contains all the necessary hardware to run a computer operating system. The board has a Central Processing Unit (CPU) as well as a Graphics Processing Unit (GPU) This low-cost single board computer provides the user with access to the General-Purpose Input/Output (GPIO) physical pins that connect to the CPU. The GPIO pins allow the user to program the physical pins on the processor and use those pins as either an input or an output.  The Raspberry Pi 4 is the newest version of the board and will remain in production until at least January 2026.

![pi4](assets\img\pi4.png)

## 1.1. Pi On-Board Components

The [Pi has the following components built into the board](https://www.raspberrypi.com/products/raspberry-pi-4-model-b/specifications/)
- Broadcom BCM2711, Quad core ARM 64 bit processor
- RAM options of 2GB, 4GB, 8GB
- Wireless and Bluetooth connectivity
- Ethernet port
- USB 3.0 and USB 2.0
- 2 x micro-HDMI connectors
- Micro-SD card slot
- USB-C for 5V power


## 1.2. Input monitoring with the Pi

The 40-pin GPIO header found on the Pi enables the connection of the CPU monitor various types of inputs. Most of the pins on the header can be programed as an input or an output. 
The input pins can be used to monitor the state of a switch or value of a sensor. 

![pi_input](assets\img\pi_input.png)

| :----: |
| <b>Fig.2 - GPIO as an Input</b>|



## 1.3. GPIO Header

The GPIO header on the Pi has 40 male pins spaced 2.54 mm / 0.1 in apart. The Pi uses two distinct pin naming conventions. Understanding the pin numbering is critical to correctly working with the GPIO. The physical pin numbering (BOARD) is shown in the center rectangle of Figure 1. The odd physical pins are on the left side and the even pins are on the right side. The pins are numbered in sequence from left to right. The second numbering system uses the Broadcom (BCM) CPU pin sequence. Most of these pins are labeled with a GPIO on the front of the name. They are not sequenced on the board in any discernible pattern.  The following bullet points show an example of the two numbering systems.
- BOARD pin 11 is the same as BCM pin 17 which is labeled GPIO17
- BOARD pin 13 is the same as BCM pin 27 which is labeled as GPIO27
The numbering systems used by the Pi can be a bit confusing. Open source programs found online may use either system. The program will identify which of the systems that is used in the code.  Code Snippet 1 for BCM and Code Snippet 2 for BOARD. This paper and all associated code will use the BOARD numbering system. More Pi GPIO pin information can be found at https://pinout.xyz/. 



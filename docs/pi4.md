---
layout: default
title: Lab 1 - Introduction to the Raspberry Pi
nav_order: 1
---
<p align="center">
<iframe width="560" height="315" src="https://www.youtube.com/embed/TrnCnbPjTJU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

</p>

# 1. Raspberry Pi - A Single Board Computer

The **[Raspberry Pi 4](https://www.raspberrypi.com/products/raspberry-pi-4-model-b/)**
is a credit card size computer that contains all the necessary hardware to run a computer operating system. The board has a Central Processing Unit (CPU) as well as a Graphics Processing Unit (GPU) This low-cost single board computer provides the user with access to the General-Purpose Input/Output (GPIO) physical pins that connect to the CPU. The GPIO pins allow the user to program the physical pins on the processor and use those pins as either an input or an output.  The Raspberry Pi 4 is the newest version of the board and will remain in production until at least January 2026.



![pi4](assets\img\pi4.png)
<p align=right><b>Fig.1 - Raspberry Pi 4 Model B - Image By<a href="https://www.raspberrypi.com/products/raspberry-pi-4-model-b/"> Raspberry Pi</a></b></p>

## 1.1. Pi On-Board Components

The **[Pi has the following components built into the board](https://www.raspberrypi.com/products/raspberry-pi-4-model-b/specifications/)**
- Broadcom BCM2711, Quad core ARM 64 bit processor
- RAM options of 2GB, 4GB, 8GB
- Wireless and Bluetooth connectivity
- Ethernet port
- USB 3.0 and USB 2.0
- 2 x micro-HDMI connectors
- Micro-SD card slot
- USB-C for 5V power

### 1.1.1. Central Processing Unit (CPU)

The CPU on the Pi is the used to execute instructions. The CPU is given instruction by a program that is written in a language called Python.  **[What does a CPU actually do?](https://www.digitaltrends.com/computing/what-is-a-cpu/)**




### 1.1.2. Circuit Traces

The Pi's components are mounted on a **[printed circuit board (PCB)](https://www.youtube.com/watch?v=H9pGbLJknDk)**. The PCB has small conductive paths that connect the components to each other. These conductive paths replace the need for traditional electrical wiring.



![chip](assets\img\chip-6074903.jpg)
<p align=right><b>Fig.2 - Circuit Traces - Image by <a href="https://pixabay.com/users/fabersam-98886/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=6074903">Samuel Faber</a> from <a href="https://pixabay.com/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=6074903">Pixabay</a></b></p>


### 1.1.3. General Purpose Input Output (GPIO)

The 40-pin GPIO header found on the Pi enables easy access to the CPU pins. The male header pins are spaced 2.54mm (0.1 inches) apart. The pins are used to make an CPU pins electrically accessible. We will cover the GPIO in detail in future pages.

![chip](assets\img\chip-6074903.jpg)
<p align=right><b>Fig.3 - Raspberry Pi 4 GPIOy</b></p>

## 1.2. Input monitoring with the Pi

The 40-pin GPIO header found on the Pi enables the connection of the CPU monitor various types of inputs. Most of the pins on the header can be programed as an input or an output. 
The input pins can be used to monitor the state of a switch or value of a sensor. 

![pi_gpio](assets\img\piGPIO.jpg)
<p align=right><b>Fig.4 - GPIO as an Input</b></p>



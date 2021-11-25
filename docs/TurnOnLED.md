---
layout: default
title: Lab 2 - Turn On An LED
nav_order: 2
---
<p align="center">
TODO video
</p>

# 2. Light Emitting Diode (LED)

An [LED](https://learn.adafruit.com/all-about-leds/what-are-leds-used-for) is an electronic device that illuminates when current passes through it in the "correct direction", also known as a forward-bias. 

When the positive terminal of a battery is applied to the anode (+) and the negative terminal of the battery is applied to the cathode (-), current flows through the LED (forward bias). Voltage applied in the other direction results in no current flow (reverse bias). 

![LED](assets\img\led-on.png)



<p align=right>
<b>Fig.1 - Light Emitting Diode - Image by 
<a href="https://pixabay.com/users/openclipart-vectors-30363/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=2023979">
OpenClipart-Vectors</a> 
from 
<a href="https://pixabay.com/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=2023979">
Pixabay
</a></b></p>

## 2.1 Parts of an LED

The anode (+) is typically the longer side of an LED (see Side Profile). The cathode (-) is typically the flat side of an LED (see Top Profile). The schematic symbol for an LED is a diode with arrows representing the light emitting component of an LED (see LED Schematic Symbol)


![LED Symbol](assets\img\LEDx3.jpg)


<p align=right><b>Fig.2 - Light Emitting Diode Symbol - Original Image by <a href="https://upload.wikimedia.org/wikipedia/commons/5/52/%2B-_of_LED_2.svg">Adam850</a> from <a href="https://commons.wikimedia.org/wiki/File:%2B-_of_LED_2.svg">Wikimedia</a></b></p>


## 2.1. Pi On-Board Components

The **[Pi has the following components built into the board](https://www.raspberrypi.com/products/raspberry-pi-4-model-b/specifications/)**
- Broadcom BCM2711, Quad core ARM 64 bit processor
- RAM options of 2GB, 4GB, 8GB
- Wireless and Bluetooth connectivity
- Ethernet port
- USB 3.0 and USB 2.0
- 2 x micro-HDMI connectors
- Micro-SD card slot
- USB-C for 5V power

## 2.2. Central Processing Unit (CPU)

The CPU on the Pi is the used to execute instructions. The CPU is given instruction from memory using content saved in storage. This storage content is written in a language called Python.  **[What does a CPU actually do?](https://www.digitaltrends.com/computing/what-is-a-cpu/)**

![CPU](assets\img\cpu.jpg)
<p align=right><b>Fig.2 - Central Processing Unit</b></p>

### 2.2.1. Circuit Traces

The Pi's components are mounted on a **[printed circuit board (PCB)](https://www.youtube.com/watch?v=H9pGbLJknDk)**. The PCB has small conductive paths that connect the components to each other. These conductive paths replace the need for traditional electrical wiring.

![chip](assets\img\chip-6074903.jpg)
<p align=right><b>Fig.3 - Circuit Traces - Image by <a href="https://pixabay.com/users/fabersam-98886/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=6074903">Samuel Faber</a> from <a href="https://pixabay.com/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=6074903">Pixabay</a></b></p>


## 2.3. Memory and Storage

The Pi has options for 2GB, 4G, and 8GB memory. This memory is Random Access Memory (RAM). RAM is volatile meaning it is erased as soon as the power is turned off. RAM is used by the CPU to access the programming instructions found in storage.

A micro-SD card is used for data storage on the pi. The operating system (OS) and all of the programs are stored on the micro-SD card. The micro-SD card can be removed and inserted into a different Pi 4. The OS and all the programs can be used in a similar manner on any other Pi 4.

![pi_gpio](assets\img\StorageMemory.jpg)
<p align=right><b>Fig.4 - Memory vs Storage</b></p>



## 1.4. General Purpose Input Output (GPIO)

The 40-pin GPIO header found on the Pi enables easy access to the CPU pins. The male header pins are spaced 2.54mm (0.1 inches) apart. The pins are used to make an CPU pins electrically accessible. We will cover the GPIO in detail in future pages.

![pi_gpio](assets\img\piGPIO.jpg)
<p align=right><b>Fig.5 - Raspberry Pi 4 GPIO</b></p>

## 1.5. Input monitoring with the Pi

Most of the pins on the GPIO can be programmed to operate as an input monitor. The pin can monitor the condition of a switch (on/off) or the position of a sensor (5 degrees, 20 degrees, 70 degrees ...) 

![pi_gpio](assets\img\pi_input.png)
<p align=right><b>Fig.6 - Input</b></p>

## 1.6. Output control with the Pi

Most of the pins on the GPIO can be programmed to operate as an output. The pin can be used to turn on a light or vary the speed of a motor.

![pi_gpio](assets\img\output.jpg)
<p align=right><b>Fig.7 - Output</b></p>



## 1.7. Programming Language - Python

[Python](https://www.python.org/) is a popular programming language. Computers communicate using a series of 1's and 0's. It would be challenging to remember the sequence of 1's and 0's for every set of instruction that you want the computer to run. Software engineers use high level languages (HLL), like Python, to write programs that are more readable. These HLLs are converted into binary in order for the computer to run the instructions.

```python
# Python Example -- multiply two numbers

first_number = 100
second_number = 50

answer = first_number * second_number

print(answer)

```

## 1.8. Running Programs on the Pi

The Pi uses instructions from storage that are written in python. Those instructions are written to memory when the Pi is given the command to run the program. The CPU fetches the instructions from memory, performs the needed calculations and returns the results. The CPU and Memory use the information from the GPIO to identify the state of any pins designated as inputs. The information gathered from the input pins is used by memory to modify instructions. 

![pi_gpio](assets\img\ComputerProcessor.jpg)
<p align=right><b>Fig.8 - Processes of running a program</b></p>


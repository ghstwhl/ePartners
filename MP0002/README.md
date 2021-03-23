# USB Module U Disk Module CH376 CH376s Storage

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

CH376 is common a USB bus interface chip, with 8 bit data bus and reading , writing and chip select
lines and interrupt output , can easily attached to the system bus of the single chip microcomputer
/DSP/MCU/MPU controller. In the USB host mode , CH376 also provides a serial communication
mode, through the serial input, serial output and interrupt output connected with the MCU
/DSP/MCU/MPU.
The "CH376S/CH375 USB read/write module" has a CH376S/CH375 chip onboard which does most
of the hard work for you. All you have to do is send the module some commands from the Arduino
and the CH376S/CH375 chip will do the rest. You can communicate with the module in three different
ways:
• Parallel communication
• SPI communication
• and Serial (UART) communication.
CH376 is used as file manage control chip, used to MCU system read/write file in USB Flash Driveor
SD card. CH376 supports USB-Device Mode and USB-HOST Mode. Set the basic firmware of USB
communication protocol in the inner. It is also set firmware of special communication protocol to deal
with Mass-Storage devices, communication interface firmware of SD card, FAT16, FAT32 and FAT12
file system manage firmware in the inner. It supports common USB storage devices (contains USB
Flash Drive/USB hard disk/USB Flash memory/USB read card) and SD cards (contain SD card with
standard capacity and HC-SD card with high capacity, MMC card and TF card compatible with
protocol).
CH376 supports three communication interfaces: 8-bit parallel, SPI interface or asynchronism serial
interface. DSP/MCU/MPU etc. controller via the any interface of them to control CH376 chip, storage
and get file in USB Flash Drive or SD card, or communication with computer.
The USB-DEVICE Mode of CH376 is totally compatible with CH372, the USB-HOST Mode of CH375
is basically compatible with CH375.

---

## Features (Specifications)

| Features                         |                                                              |
| -------------------------------- | ------------------------------------------------------------ |
| Support Formats                  | FAT12, FAT16, FAT32                                          |
| Communication interfaces         | 8-bit parallel, SPI interface, asynchronism serial Interface |
| 2x8 connection head              | convenient to hang with MCU                                  |
| Jumper option                    | work in parallel or serial mode                              |
| USB status indicator light       |                                                              |
| Plate load                       | LDO 3.3V 1117                                                |
| Maximum current                  | 800mA                                                        |
| Power supply by the target board | 5V                                                           |
| Oscilicator                      | 12MHZ crystal                                                |
| Size                             | 47 x 27mm                                                    |

---

## Pins

![alt text](https://bit.ly/3d0cQJZ)

---

## Test

-   [Tutorial](https://github.com/djuseeq/Ch376msc)
-   [Tutorial Video I](https://www.youtube.com/watch?v=fCBS3jQzQj0)
-   [Tutorial Video II ](http://bit.ly/CH376-YouTube)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [Datasheet](https://drive.google.com/file/d/1-6tky01XxXkajA2Zg9Mn4eIM3suVJS68/view)

-   [More features](http://wch-ic.com/products/CH376.html)

-   **to be updated..**

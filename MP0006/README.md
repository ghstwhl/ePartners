# Reading and Writing Module SD Card Module Slot Socket Reader

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The module (SD Card Adapter) is a SD card reader module, through the file system and the SPI interface driver, MCU to complete the file system to read and write SD card.
Users can directly use IDE comes with an SD card to complete the library card initialization and read-write.

---

## Features (Specifications)

| Features                |                                               |
| ----------------------- | --------------------------------------------- |
| Supports card type      | SD Card                                       |
| Communication interface | standard SPI interface                        |
| Control Interface       | GND, VCC, MISO, MOSI, SCK, CS (GND to ground) |
| Power supply            | VCC                                           |
| SPI Bus                 | MISO, MOSI, SCK                               |
| Chip select signal pin  | CS                                            |
| Positioning hole        | 2 x M2 screws positioning hole diameter       |

---

## Pins

| SD Card Module | Arduino Uno | Function            |
| -------------- | ----------- | ------------------- |
| 5V             | 5V          | Power               |
| CS             | D10         | Chip Select         |
| MOSI           | D11         | Master Out Slave In |
| SCK            | D13         | Serial Clock        |
| MISO           | D12         | Master In Slave Out |
| GND            | GND         | Ground Connection   |

---

## Test

-   [Tutorial I](http://bit.ly/Guide-to-SD-Card-Module)
-   [Tutorial II](https://bit.ly/3tO48pk)
-   [Tutorial III](https://dronebotworkshop.com/sd-card-arduino/)

-   [Tutorial Video I](https://www.youtube.com/watch?v=finwzEU1CB0)
-   [Tutorial Video II](https://www.youtube.com/watch?v=oTXi6kYg0D4)

**to be updated..**

---

## Troubleshooting

-   [Common Problem with Arduino](https://www.youtube.com/watch?v=9xsLfjCArX8)

**to be updated..**

---

## References

-   **to be updated..**

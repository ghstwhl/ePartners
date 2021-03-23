# Micro SD card mini TF card reader-module SPI interfaces with level converter

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The module (MicroSD Card Adapter) is a Micro SD card reader module, through the file system and the SPI interface driver, MCU to complete the file system to read and write MicroSD card.
Users can directly use IDE comes with an SD card to complete the library card initialization and read-write.

---

## Features (Specifications)

| Features                                         |                                                      |
| ------------------------------------------------ | ---------------------------------------------------- |
| Supports card type                               | Micro SD                                             |
|                                                  | Micro SDHC card (high speed card)                    |
| Level conversion circuit board (Interface lever) | 5V or 3.3V                                           |
| Communication interface                          | standard SPI interface                               |
| Control Interface                                | GND, VCC, MISO, MOSI, SCK, CS (GND to ground)        |
| Power supply                                     | VCC                                                  |
| SPI Bus                                          | MISO, MOSI, SCK                                      |
| Chip select signal pin                           | CS                                                   |
| 3.3V voltage regulator circuit                   | 3.3V level converter chip (LDO regulator output)     |
|                                                  | Micro SD card supply                                 |
| Level conversion circuit                         | Micro SD card => 3.3V                                |
|                                                  | MISO signal => 3.3V                                  |
|                                                  | General AVR microcontroller system (Read the signal) |
| Micro SD card connector                          | Self-bomb deck                                       |
|                                                  | Easy card insertion                                  |
| Positioning hole                                 | 4 x M2 screws positioning hole diameter              |

---

## Pins

| SD card Module | Arduino |
| -------------- | ------- |
| VCC            | VCC     |
| MISO           | D12     |
| MOSI           | D11     |
| SCK            | D13     |
| CS             | D10     |

---

## Test

-   [Tutorial I](https://www.electronics-lab.com/project/interfacing-arduino-micro-sd-card-module/)
-   [Tutorial II](https://lastminuteengineers.com/arduino-micro-sd-card-module-tutorial/)
-   [Tutorial Video I](https://www.youtube.com/watch?v=PQhQfww-qGQ)
-   [Tutorial Video II](https://youtu.be/sS_oW81NweI)
-   [Tutorial Video III](https://www.youtube.com/watch?v=5Dp-XatLySM)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [Another type SD card](https://randomnerdtutorials.com/guide-to-sd-card-module-with-arduino/)

-   **to be updated..**

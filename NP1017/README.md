# Dot Matrix Module MAX7219 Microcontroller 4 In One Display with 5P Line

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The MAX7219 is a popular and flexible 7-segment, bar graph and dot matrix common cathode LED driver that supports many functions for controlling LED displays.

The driver provides flexible individual LED control as well as basic functions such as turning the display ON/OFF and adjusting the LED brightness.

The MAX7219 communicates with an MCU via a 3-wire SPI bus. Once the display is updated by the MCU, the MAX7219 then takes care of all the work of keeping the display refreshed, so it removes that overhead from the MCU which can be off doing other more important things.

---

## Features (Specifications)

| Features (Specifications) |                  |
| ------------------------- | ---------------- |
| Operating voltage         | 5 V              |
| Display driver            | MAX7219 x 4      |
| Brightness levels         | 16               |
| Display dimensions        | 32 x 128 x 15 mm |
| Pixels                    | 8×32, ⌀ 3 mm     |

---

## Pins

![alt text](https://bit.ly/3gCkw8P 'Pinout')

### Input connector

| Pin name | Description           |
| -------- | --------------------- |
| VCC      | 5V(+)                 |
| GND      | Common Ground(-)      |
| DIN      | Data In (Digital)     |
| CS/LOAD  | Chip Select (Digital) |
| CLK      | Clock pin (Digital)   |

### Output connector

| Pin name | Description                                           |
| -------- | ----------------------------------------------------- |
| VCC      | 5V(+)                                                 |
| GND      | Common Ground(-)                                      |
| DOUT     | Data Out (Connects to the DIN pin of the next module) |
| CS/LOAD  | Connects to CS / LOAD on next module                  |
| CLK      | Connects to CLK on next module                        |

---

## Test

-   [Tutorial I](https://bit.ly/3eowNuW)
-   [Tutorial II](https://bit.ly/3xc7oxb)
-   [Tutorial III](https://bit.ly/3tLeQ07)

-   [Tutorial Video I](https://youtu.be/SIlLj4thyso)
-   [Tutorial Video II](https://youtu.be/mvfh1pXTvN4)
-   [Tutorial Video III](https://youtu.be/TaqSaYI0aLI)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [MAX7219 Datasheet](https://bit.ly/3tLLBdk)
-   [Parola](https://github.com/MajicDesigns/MD_Parola)

**to be updated..**

#

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The CNC Shield V3.0 allows you to build a engraving machine, 3D printer, mini CNC and other similar devices using your Arduino. It is designed as a shield and can plug on top of an Arduino requiring no external connections and wiring. There are 4 slots on the board for plugging in stepper motor drive module which can drive 1 stepper motor each. Controlling each step stepper motor requires only two IO pins on the Arduino. Just insert this Arduino CNC Shield V3.0 onto an Arduino UNO, and install the GRBL firmware, you can then quickly build a DIY CNC engraving machine.

---

## Features (Specifications)

| Features (Specifications)                                                                                                                                 |     |
| --------------------------------------------------------------------------------------------------------------------------------------------------------- | --- |
| Coolant enable                                                                                                                                            |
| Uses removable Pololu A4988 compatible stepper drivers. (A4988, DRV8825 and others) (Not Included)                                                        |
| Jumpers to set the Micro-Stepping for the stepper drivers. (Some drivers like the DRV8825 can do up to 1/32 micro-stepping )                              |
| Compact design.                                                                                                                                           |
| Stepper Motors can be connected with 4 pin molex connectors or soldered in place.                                                                         |
| Runs on 12-36V DC. (At the moment only the Pololu DRV8825 drivers can handle up to 36V so please consider the operation voltage when powering the board.) |
| Please note that this is an unassembled kit and needs soldering.                                                                                          |
| GRBL 0.9 compatible. (Open source firmware that runs on an Arduino UNO that turns G-code commands into stepper signals)                                   |
| PWM Spindle and direction pins                                                                                                                            |
| 4-Axis support (X, Y, Z , A-Can duplicate X,Y,Z or do a full 4th axis with custom firmware using pins D12 and D13)                                        |
| 2 x End stops for each axis (6 in total)                                                                                                                  |

---

## Pins

| ![alt text](https://bit.ly/3w7CQfv 'CNC shield') |
| ------------------------------------------------ |

---

## Test

-   [Tutorial for DRV8825](https://bit.ly/3fn2cjw)
-   [Tutorial Video for DRV8825](https://youtu.be/DZcrrFcs4N4)

-   [Tutorial for A4988](https://bit.ly/31AK2CC)
-   [Tutorial Video for A4988](https://youtu.be/TMK_fLgpESQ)

-   [Instructions for 3020CNC](https://bit.ly/3u2Gm8Q)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

**to be updated..**

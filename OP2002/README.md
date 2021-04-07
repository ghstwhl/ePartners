# Logic Level Converter - 4 Channel Bi-Directional 5V to 3.3V

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

Do you have a 3.3V I2C or SPI sensor that might go up in smoke if connected to a 5V Arduino? Or a 5V device that needs a workaround to be compatible with your 3.3V Raspberry Pi 4, Raspberry Pi Zero, RedBoard Turbo, RedBoard Turbo or Arduino Due?

To get over this obstacle you need a device that can shift 3.3V up to 5V or 5V down to 3.3V. This is called logic level shifting. Level shifting is a dilemma so common we designed a simple PCB assembly to make interfacing devices a little easier: the Bi-Directional Logic Level Converter.

---

## Features (Specifications)

| Features (Specifications)                                        |
| ---------------------------------------------------------------- |
| 4 channels can convert up to 4 logic signals                     |
| Can convert between 1.8V, 2.8V, 3.3V and 5V logic circuits       |
| Bi-directional so can work with bi-directional buses such as I2C |
| Utilizes N-Ch MOSFET transistors for level translation           |

---

## Pins

| Pin name  | Functions    | Description                                                             |
| --------- | ------------ | ----------------------------------------------------------------------- |
| HV        | High voltage | Must be higher voltage than LV. Typically tied to 5V                    |
| LV        | Low voltage  | Must be lower voltage than HV. Typically tied to 3.3V                   |
| GND       | Ground (x2)  | Can be used to pass a ground between the two different voltage circuits |
| HV1 / LV1 | Channel 1    |                                                                         |
| HV2 / LV2 | Channel 2    |                                                                         |
| HV3 / LV3 | Channel 3    |                                                                         |
| HV4 / LV4 | Channel 4    |                                                                         |

## Test

-   [Tutorial I](https://bit.ly/3wHqOd9)
-   [Tutorial II](https://bit.ly/3urpsRE)
-   [Tutorial II]()

-   [Tutorial Video I]()
-   [Tutorial Video II]()
-   [Tutorial Video III]()

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [Bi-directional Logic Level Converter](https://bit.ly/3fNl1fT)
-   [Logic Level shifting](https://bit.ly/3uqTYLq)

**to be updated..**

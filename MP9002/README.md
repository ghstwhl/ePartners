# current / power monitoring sensor -I2C interface Bi-directional INA219

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The INA219 based Current sensor module CJMCU-219 is an I2C interface based zero drift and bi-directional current/power monitoring module. It can sense shunt voltage, current, and power at the same time and submit the data via I2C protocol.

---

## Features (Specifications)

| Features (Specifications)                                                     |
| ----------------------------------------------------------------------------- |
| Power Input: 3.0V-5.5V                                                        |
| Up to +26V target voltage                                                     |
| 0.1 ohm 1% 2W current sense resistor                                          |
| Up to ±3.2A current measurement, with ±0.8mA resolution                       |
| Senses Bus Voltages from 0 to 26 V                                            |
| 2C- or SMBus-compatible interface                                             |
| Up to 128 samples can be averaged to achieve filtering in noisy environments. |
| Board Dimension: 0.8 x 0.9 inch (l x w x h)                                   |

---

## Pins

| ![alt text](https://bit.ly/3wb5o7F 'pinout') | ![alt text](https://bit.ly/3rwZqe3 'pinout') |
| -------------------------------------------- | -------------------------------------------- |

| Pin Name | Function            | Comments                                            |
| -------- | ------------------- | --------------------------------------------------- |
| VIN-     | Sensed Input line - | Same connection available on the interface section. |
| VIN+     | Sensed Input line + | Same connection available on the interface section. |
| VCC      | Input voltage       | For powering up the module                          |
| GND      | GND                 |                                                     |
| SCL      | I2C SCL             |                                                     |
| SDA      | I2C SDA             |                                                     |

---

## Test

-   [Tutorial I](https://diyi0t.com/ina219-tutorial-for-arduino-and-esp/)
-   [Tutorial II](https://electropeak.com/learn/interfacing-ina219-current-sensor-module-with-arduino/)
-   [Tutorial III](https://bit.ly/3fmpJkx)

-   [Tutorial Video I](https://youtu.be/FXQoZbvM3Kw)
-   [Tutorial Video I](https://youtu.be/JWUKFLCX5Os)
-   [Tutorial Video I](https://youtu.be/WI4pWs0DYPU)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [INA219 Datasheet](https://bit.ly/3w78xFF)

**to be updated..**

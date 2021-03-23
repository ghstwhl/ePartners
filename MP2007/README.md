# PCF8574 I/O Expansion Board I2C-Bus

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The PCF8574 module is used to expand the input/output (I/O) ports over an I2C connection with 8-bit input/outputs. Use with microcontrollers (Arduino) over the I2C serial interface.

The device features an 8-bit bidirectional I/O port (P0–P7), including latched outputs with high current drive capability for directly driving LEDs. Each bidirectional I/O can be used as an input or output without the use of a data-direction control signal.

Three on-board jumpers allow for the selection of up to 8 I2C addresses, allowing up to 8 modules for 64 I/O pins can be connected to the same I2C interface. The module also features convenient input and output headers at each end so that additional modules can simply be daisy-chained without the need for additional wires.

To use this module with standard Arduino boards, download the HCPCF8574 library and example sketches.

---

## Features (Specifications)

| Features (Specifications)                                             |
| --------------------------------------------------------------------- |
| 8 bi-directional data lines                                           |
| Loop-thru feature allows expansion of up to 8 modules / 64 data lines |
| I2C interface with jumper adjustable addresses                        |
| Interrupt output capability                                           |
| 3.3V and 5V compatible.                                               |

---

## Pins

| PCF08574 | Arduino         |
| -------- | --------------- |
| VCC      | 3.3V or 5V      |
| GND      | GND             |
| SDA      | SDA (I2C Data)  |
| SCL      | SCL (I2C Clock) |

| Address(Hex) | A2   | A1   | A0   |
| ------------ | ---- | ---- | ---- |
| 0x20         | LOW  | LOW  | LOW  |
| 0x21         | LOW  | LOW  | HIGH |
| 0x22         | LOW  | HIGH | LOW  |
| 0x23         | LOW  | HIGH | HIGH |
| 0x24         | HIGH | LOW  | LOW  |
| 0x25         | HIGH | LOW  | HIGH |
| 0x26         | HIGH | HIGH | LOW  |
| 0x27         | HIGH | HIGH | HIGH |

![alt text](https://bit.ly/318SFnO 'PCF8574')

---

## Test

-   [Tutorial I](https://www.instructables.com/Arduino-and-PCF8574-IO-Expander-Binary-Counter-and/)
-   [Tutorial II](https://www.instructables.com/PCF8574-GPIO-Extender-With-Arduino-and-NodeMCU/)
-   [Tutorial III](https://www.electronicshub.org/interfacing-pcf8574-with-arduino/)
-   [Tutorial IV](http://bit.ly/2QRSNkY)

-   [Tutorial Video I](https://youtu.be/-CXSEWlMYFs)
-   [Tutorial Video II](https://youtu.be/mXMkgQf3fqU)
-   [Tutorial Video III](https://youtu.be/kQZU8kE3ksU)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [Datasheet](http://bit.ly/pcf8574-Datasheet)

-   **to be updated..**

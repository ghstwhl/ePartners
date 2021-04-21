# TTL to RS485 Module UART Port Converter

## Table of Contents

- [Descriptions](#descriptions)
- [Features](#features)
- [Pins](#pins)
- [Test](#test-code)
- [Troubleshooting](#troubleshooting)
- [References](#references)

---

## Descriptions

This is a module that allows the TTL interface of the microcontroller to be transferred to the RS485 module. It is generally used for industrial automation. This module adds lightning protection design and anti-jamming design. When we use it in the field and carry out long distance transmission, we can Connect the GND end of the module to the ground so that lightning protection and anti-interference can be achieved.
It uses a standard 2.54 mm pitch design. If you want to make the second development will be more convenient. It has 120 ohm matching resistance, shorted R0 can, it is recommended that users in the long distance transmission shorted.
It supports communication between multiple microcontrollers, allowing up to 128 devices on the bus. It can be hot-swappable, in order to prevent signal interference, it carried out a large area of copper, the effect is very good.

---

## Features (Specifications)

| Features                        |                                            |
| ------------------------------- | ------------------------------------------ |
| Operating voltage               | compatible with 5.0V                       |
| Support baud rate               | 110-256000bps                              |
| Operating temperature           | -40 ℃ to + 85 ℃                            |
| Communication signal            | compatible with 3.3V and 5.0V              |
| RXD, TXD signal indicator light | monitor send and receive status            |
| Transmission distance           | it is recommended to use in the 800 meters |

---

## Pins

![alt text](https://bit.ly/3ene5Um "Pin out")

| Pin | Description                                                 |
| --- | ----------------------------------------------------------- |
| VCC | Vcc – Connect to 3.3V or 5V to match MCU power              |
| RXD | Receive Data – Connects to RXD TTL input on MCU             |
| TXD | Transmit Data – Connects to TXD TTL output on MCU           |
| GND | Ground. Connects to ground on MCU                           |
| A+  | Data ‘A’ Non-Inverted Line. Connects to A+ on other modules |
| B-  | Data ‘B’ Inverted Line. Connects to B- on other modules     |
| GND | Ground                                                      |

---

## Test

- [Tutorial](https://bit.ly/3v8Jot0)

- [Tutorial Video](https://youtu.be/Oq019vxRj54)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

**to be updated..**

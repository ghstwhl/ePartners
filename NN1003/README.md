# MAX485 RS485 Transceiver Module

## Table of Contents

- [Descriptions](#descriptions)
- [Features](#features)
- [Pins](#pins)
- [Test](#test-code)
- [Troubleshooting](#troubleshooting)
- [References](#references)

---

## Descriptions

This low power transceiver module is based on the Maxim MAX485 IC to allow serial communication over very long cable runs (up 4000 feet / 1200 meters). Serial data can be transmitted in both directions (half duplex) at a data rate up to 2.5Mbps. The modules operate from a standard 5V power supply and use 5V logic levels allowing them to be interfaced to the hardware serial ports of microcontrollers such as Arduino/PIC etc. Direction of communication can be controlled with just one digital pin (see diagram). It is also possible to connect multiple modules together for communication between 2 or more devices. For even greater distances two modules can be configured as a repeater.

Each module contains one driver and one receiver. Drivers are short-circuit current limited and are protected against excessive power dissipation by thermal shutdown circuitry that places the driver outputs into a high-impedance state. The receiver input has a fail-safe feature that guarantees a logic-high output if the input is open circuit.

Data connections to the modules are provided by a standard 0.1" pitch header pins which can also be soldered into standard prototyping PCB and breadboards. Screw terminals provide convention connection to the actual data cable.

---

## Features (Specifications)

| Features                                         |
| ------------------------------------------------ |
| Use MAX485 Interface chip                        |
| Uses differential signaling for noise immunity   |
| Distances up to 1200 meters                      |
| Speeds up to 2.5Mbit/Sec                         |
| Multi-drop supports up to 32 devices on same bus |
| Red power LED                                    |
| 5V operation                                     |

---

## Pins

![alt text](https://bit.ly/3dw5I9N "Pin out")

| Pins |                                                               |
| ---- | ------------------------------------------------------------- |
| VCC  | 5V                                                            |
| A    | Non-inverting Receiver Input and No-ninverting Driver Output. |
| B    | Inverting Receiver Input and Inverting Driver Output          |
| GND  | 0V                                                            |
| R0   | Receiver Output (to Rx pin of microcontroller)                |
| RE   | Receiver Output Enable (Low to enable)                        |
| DE   | Driver Output Enable (high to enable)                         |
| DI   | Driver Input (to Tx pin of microcontroller)                   |

---

## Test

- [Tutorial I](https://bit.ly/3x8eeDP)
- [Tutorial II](https://bit.ly/3gjRyKV)
- [Tutorial III](https://bit.ly/2P6r8B8)

- [Tutorial Video I](https://youtu.be/sLD-2QDkCd0)
- [Tutorial Video II](https://youtu.be/Bhvap1qXcHg)
- [Tutorial Video III](https://youtu.be/GjdytbCIYSY)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

- [MAX485 Datasheet](https://bit.ly/3x8fx5H)

**to be updated..**

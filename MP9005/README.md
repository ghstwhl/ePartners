# nRF24L01 + 2.4GHz Antenna Wireless Module Mutipoint Communication 125 Channels

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The nRF24L01+ transceiver module is designed to operate in 2.4 GHz worldwide ISM frequency band and uses GFSK modulation for data transmission. The data transfer rate can be one of 250kbps, 1Mbps and 2Mbps.

---

## Features (Specifications)

| Features (Specifications)    |                                                            |
| ---------------------------- | ---------------------------------------------------------- |
| Maximum operating speeds     | up to 2Mbps,                                               |
|                              | GFSK modulation efficiency                                 |
|                              | Anti-interference ability                                  |
|                              | Particularly suitable for industrial control applications  |
| Channels                     | 125 Channels                                               |
|                              | Multi-point communication and frequency                    |
|                              | hopping to meet the communication needs                    |
| Control                      | Built-in hardware CRC error detection                      |
|                              | Multipoint communication address control                   |
| Low-power                    | 1.9 ~ 3.6V, only 1uA on Power-down mode                    |
| Built-in 2.4Ghz antenna      |                                                            |
| Software                     | Available software to set the address                      |
|                              | only received local Address                                |
|                              | when output data(Provide interrupt instruction)            |
|                              | can be directly connected to a variety of microcontrollers |
|                              | Software programming is very convenient                    |
| Voltage regulator            | Built-in                                                   |
| Standard DIP Pitch Interface | for embedded applications                                  |
| size                         | 34mm X 17mm X 1mm                                          |

---

## Pins

| ![alt text](https://bit.ly/3rtymw1 'pinout') | ![alt text](https://bit.ly/2NZVBQC 'pinout') |
| -------------------------------------------- | -------------------------------------------- |

| Pin Number | Pin Name | Abbreviation        | Function                                    |
| ---------- | -------- | ------------------- | ------------------------------------------- |
| 1          | Ground   | Ground              | Connected to the Ground of the system       |
| 2          | Vcc      | Power               | Powers the module using 3.3V                |
| 3          | CE       | Chip Enable         | Used to enable SPI communication            |
| 4          | CSN      | Ship Select Not     | This pin has to be kept high always,        |
|            |          |                     | else it will disable the SPI                |
| 5          | SCK      | Serial Clock        | Provides the clock pulse using              |
|            |          |                     | which the SPI communication works           |
| 6          | MOSI     | Master Out Slave In | Connected to MOSI pin of MCU,               |
|            |          |                     | for the module to receive data from the MCU |
| 7          | MISO     | Master In Slave Out | Connected to MISO pin of MCU,               |
|            |          |                     | for the module to send data from the MCU    |
| 8          | IRQ      | Interrupt           | It is an active low pin and is used only    |
|            |          |                     | if interrupt is required                    |

---

## Test

-   [Tutorial I](https://bit.ly/NRF24L01-tutorial)
-   [Tutorial II](https://bit.ly/NRF24L01-tutorial2)

-   [Tutorial Video I](https://youtu.be/7rcVeFFHcFM)
-   [Tutorial Video II](https://youtu.be/RGF9gpTTDHY)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [nRF24-Series](https://www.nordicsemi.com/Products/Low-power-short-range-wireless/nRF24-series)
-   [nRF24-Datasheet](https://bit.ly/3w7blCK)

**to be updated..**

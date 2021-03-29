# NRF24L01 - 2.4GHz 1100-meter long-distance NRF24L01+PA+LNA

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

| Features (Specifications)        |                                                                     |
| -------------------------------- | ------------------------------------------------------------------- |
| Voltage                          | 3-3.6V                                                              |
| Max output power                 | +20 dBm                                                             |
| Working current in transmit mode | 115mA                                                               |
| Working current in receiver mode | 45mA                                                                |
| Current in mode                  | 4.2uA                                                               |
| Operating temperature            | -20-70 degree                                                       |
| Receiver sensitivity             | -92dBm in 2Mbps mode, -95dBm in 1Mbps mode, -104dBm in 250kbps mode |
| PA growth                        | 20dB                                                                |
| LAN growth                       | 10dB                                                                |
| LAN noise figure                 | 2.6dB                                                               |
| Antenna growth                   | 2dBI                                                                |
| 2M rate                          | 520m                                                                |

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

-   [Tutorial Video I](https://youtu.be/uilIwkJGtfI)
-   [Tutorial Video II](https://youtu.be/57pdX6b0sfw)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [nRF24-Series](https://www.nordicsemi.com/Products/Low-power-short-range-wireless/nRF24-series)
-   [nRF24-Datasheet](https://bit.ly/3w7blCK)

**to be updated..**

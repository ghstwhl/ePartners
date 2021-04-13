# PCF8563 PCF8563T IIC Real Time Clock RTC Module Board

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The PCF8563 RTC Board provides the real-time clock/calendar function, which can be driven by a battery on board and works independently even when the MCU is turned off.

The PCF8563 RTC Board features I2C pinheader on one side, and I2C connector on the opposite side. Hence, it's more flexible to connect the board to your development system. The board also supports I2C cascading, allowing the use of multi module connected to the I2C bus at the same time by connecting the pinheader and connector.

---

## Features (Specifications)

| Features (Specifications)                                                                                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Provides year, month, day, weekday, hours, minutes and seconds based on 32.768 kHz quartz crystal                                                                                              |
| Century flag                                                                                                                                                                                   |
| Clock operating voltage: 1.8 V to 5.5 V                                                                                                                                                        |
| Low backup current; typical 0.25 µA at VDD = 3.0 V and Tamb = 25 °C                                                                                                                            |
| 400 kHz two-wire I2C-bus interface (at VDD = 1.8 V to 5.5 V)                                                                                                                                   |
| Programmable clock output for peripheral devices (32.768 kHz, 1024 Hz, 32 Hz and 1 Hz)                                                                                                         |
| Alarm and timer functions                                                                                                                                                                      |
| Integrated oscillator capacitor                                                                                                                                                                |
| Internal power-on reset                                                                                                                                                                        |
| I<sub>2</sup>C-bus slave address: read A3h and write A2h                                                                                                                                       |
| Open-drain interrupt pin                                                                                                                                                                       |
| ElectroStatic Discharge (ESD) protection exceeds 2000 V Human Body Model (HBM) per JESD22-A114, 200 V Machine Model (MM) per JESD22-A115 and 2000 V Charged Device Model (CDM) per JESD22-C101 |
| Latch-up testing is done to JEDEC standard JESD78 which exceeds 100 mA                                                                                                                         |

---

## Pins

![alt text](https://bit.ly/2QeNxMK 'RTC')

| Pin name | Description     |
| -------- | --------------- |
| INT      | Interrupt ouput |
| COT      | Clock output    |
| VCC      | +5V             |
| GND      | Ground(-)       |
| SDA      | Serial Data     |
| SCL      | Serial Clock    |

---

## Test

-   [Tutorial I](https://bit.ly/3wPDvm6)
-   [Tutorial II](http://bit.ly/PCF8563-RTC)
-   [Tutorial III](https://bit.ly/3tjOrq4)

-   [Tutorial Video I](https://youtu.be/5g67CtiTRVA)
-   [Tutorial Video II](https://youtu.be/NEbl6TJaG-o)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [PCF8563 Datasheet](https://bit.ly/3g6B48A)

**to be updated..**

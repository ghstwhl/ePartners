# DS3231 AT24C32 IIC Module Precision Real Time Clock Module

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

At the heart of the module is a low-cost, extremely accurate RTC chip from Maxim – DS3231. It manages all timekeeping functions and features a simple two-wire I2C interface which can be easily interfaced with any microcontroller of your choice.

The chip maintains seconds, minutes, hours, day, date, month, and year information. The date at the end of the month is automatically adjusted for months with fewer than 31 days, including corrections for leap year (valid up to 2100).

The clock operates in either the 24-hour or 12-hour format with an AM/PM indicator. It also provides two programmable time-of-day alarms.

The other cool feature of this board comes with SQW pin, which outputs a nice square wave at either 1Hz, 4kHz, 8kHz or 32kHz and can be handled programmatically. This can further be used as an interrupt due to alarm condition in many time-based applications.

---

## Features (Specifications)

| Features (Specifications)                                                         |
| --------------------------------------------------------------------------------- |
| RTC counts seconds, minutes, hours and year                                       |
| Accuracy: +2ppm to -2ppm for 0ºC to +40ºC , +3.5ppm to -3.5ppm for -40ºC to +85ºC |
| Digital temperature sensor with ±3ºC accuracy                                     |
| Two Time-of-day alarms                                                            |
| Programmable square wave output                                                   |
| Register for Aging trim                                                           |
| 400Khz I2C interface                                                              |
| Low power consumption                                                             |
| Automatic power failure battery switch circuitry                                  |
| CR2032 battery backup with two to three year life                                 |
| Potable size                                                                      |
| Operating voltage of DS3231 MODULE: 2.3V – 5.5V                                   |
| Can operate on LOW voltages                                                       |
| Consumes 500nA on battery backup                                                  |
| Maximum voltage at SDA , SCL : VCC + 0.3V                                         |
| Operating temperature: -45ºC to +80ºC                                             |

---

## Pins

![alt text](https://bit.ly/3tcPvvP 'RTC')

| Pin name | Description                           |
| -------- | ------------------------------------- |
| VCC      | Connected to positive of power source |
| GND      | Connected to ground                   |
| SDA      | Serial Data pin (I2C interface)       |
| SCL      | Serial Clock pin (I2C interface)      |
| SQW      | Square Wave output pin                |
| 32K      | 32K oscillator output                 |

---

## Test

-   [Tutorial I](https://bit.ly/3mITtcR)
-   [Tutorial II](https://bit.ly/3uMndbS)
-   [Tutorial III](https://bit.ly/32bhuQp)

-   [Tutorial Video I](https://www.youtube.com/watch?v=E6wkvTG2Ofs)
-   [Tutorial Video II](https://youtu.be/BM3A7w3bhqM)
-   [Tutorial Video III](https://youtu.be/7hBtXdoaAOY)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [DS3231 Datasheet](https://bit.ly/3e3Etmi)

**to be updated..**

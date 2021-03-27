# FM Stereo Radio Module 5V TEA5767 76-108MHZ + Cable Antenna

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The TEA5767 module is a FM Stereo radio. It has a frequency range of between 76 and 108MHz. A common use for this radio is with a microcontroller using 2-wire serial protocol(i2c) to send settings.
The TEA5767HN is a single-chip electronically tuned FM stereo radio for low-voltage
applications with fully integrated Intermediate Frequency (IF) selectivity and
demodulation. The radio is completely adjustment-free and only requires a minimum of
small and low cost external components. The radio can be tuned to the European, US,
and Japanese FM bands.

---

## Features (Specifications)

| Features (Specifications)                                                                   |
| ------------------------------------------------------------------------------------------- |
| Power: 5V                                                                                   |
| FM chip module TEA5767                                                                      |
| Blue LED power indicator                                                                    |
| I2C bus communication                                                                       |
| Onboard 3.5mm audio interface                                                               |
| High sensitivity due to integrated low-noise RF input amplifier                             |
| FM mixer for conversion to IF of the US/Europe (87.5 MHz to 108 MHz)                        |
| and Japanese (76 MHz to 91 MHz) FM band                                                     |
| Preset tuning to receive Japanese TV audio up to 108 MHz                                    |
| RF Automatic Gain Control (AGC) circuit                                                     |
| LC tuner oscillator operating with low cost fixed chip inductors                            |
| FM IF selectivity performed internally                                                      |
| No external discriminator needed due to fully integrated FM demodulator                     |
| Crystal reference frequency oscillator; the oscillator operates with a 32.768 kHz clock     |
| crystal or with a 13 MHz crystal and with an externally applied 6.5 MHz reference frequency |
| Phase-locked loop (PLL) synthesizer tuning system                                           |
| I2C-bus and 3-wire bus, selectable via pin BUSMODE                                          |
| 7-bit IF counter output via the bus                                                         |
| 4-bit level information output via the bus                                                  |
| Soft mute                                                                                   |
| Signal dependent mono to stereo blend [Stereo Noise Cancelling (SNC)]                       |
| Signal dependent High Cut Control (HCC)                                                     |
| Soft mute, SNC and HCC can be switched off via the bus                                      |
| Adjustment-free stereo decoder                                                              |
| Autonomous search tuning function                                                           |
| Standby mode                                                                                |
| Two software programmable ports                                                             |
| Bus enable line to switch the bus input and output lines into 3-state mode                  |
| PCB size: 31 x 30mm                                                                         |
| With reverse polarity protection diode                                                      |
| With power output filtering sensor                                                          |
| Multi capacitor combined filter                                                             |
| Directly plug antenna interface                                                             |
| If connects with singlechip, only connect the Power Ground and two I2C communication cable. |

---

## Pins

![alt text](https://bit.ly/3w2UOQe)

| Pin Number | Description  |
| ---------- | ------------ |
| 1          | DATA         |
| 2          | CLOCK        |
| 3          | BUSMODE      |
| 4          | READ / WRITE |
| 5          | VCC          |
| 6          | GND          |
| 7          | R-OUT        |
| 8          | L-OUT        |
| 9          | MPXO         |
| 10         | ANT          |

---

## Test

-   [Tutorial I](https://www.ardumotive.com/how-to-use-the-tea5767-fm-radio-module-en.html)
-   [Tutorial II](https://www.instructables.com/How-to-use-the-TEA5767-FM-Radio-module-Arduino-Tut/)

-   [Tutorial Video I](https://youtu.be/gQZMKSKekP4)
-   [Tutorial Video II](https://youtu.be/D7P59X39N9U)
-   [Tutorial Video III](https://youtu.be/yWf9uxL6zgE)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [Datasheet](https://bit.ly/3lUDMiq)
-   [Amplication Note](https://bit.ly/3rvQq8O)

**to be updated..**

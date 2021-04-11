#

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The Sound Recorder Module uses the ISD1760 Chip to record and store voice signals. ISD1700 series recording chip is a kind of high integration, high performance chip. This module can be multiple recording, the sampling rate can be set to 6k or 8k by the on-board resistor. There are also some inside sounds to remind the user working state of the module, such as record beginning, record stopping, record erasing , etc. The recording data is stored in the FLASH, without any compression to ensure a good quality. You can easily control this module manually or by Arduino. There are some keys on the module including “REC”,”PLAY”,”EARSE”, you can control the module with these keys. The module can be also controlled by SPI, with an Arduino, you can control the detail function such as the analog path configuration, so you can integrated this module to your sound related applications.

---

## Features (Specifications)

| Features (Specifications)                                                       |
| ------------------------------------------------------------------------------- |
| Operating Voltage: Wide power supply ranges from 2.4V to 5.5V DC                |
| Dual operating modes: Standalone mode and SPI mode                              |
| Two individual input channels                                                   |
| MIC input with AGC (Automatic Gain Control)                                     |
| AnaIn (Analog input)                                                            |
| Dual output channels                                                            |
| Differential PWM Class D speaker outputs                                        |
| Configurable AUD (current) or AUX (voltage) single-ended output                 |
| Non-volatile message storage using multi-level storage (MLS)                    |
| High-quality, natural voice, and audio reproduction                             |
| Integrated message management systems for single-chip, push-button applications |

---

## Pins

| Pin name    | Description                                                                                                                  |
| ----------- | ---------------------------------------------------------------------------------------------------------------------------- |
| LED         | LED turns on during recording and blinks LED during playback, forward, and erase operations                                  |
| RST / RESET | RST input is Low, the device enters into a known state and initializes all pointers to the default state.                    |
| GND         | Ground                                                                                                                       |
| VCC         | 2.4V - 5.5V (5.0V Nominal)                                                                                                   |
| MISO        | Master In Slave Out: Data is shifted out on the falling edge of SCLK.                                                        |
| MOSI        | Master Out Slave In: In SPI slave mode, data is latched into the device on the rising edge of SCLK                           |
| SCLK        | Serial Clock: Clock of the SPI interface.                                                                                    |
| SS          | Slave Select: This input, when low, selects the device as a slave device and enables the SPI interface.                      |
| GND         | Ground                                                                                                                       |
| AnaIn       | AnaIn: Auxiliary analog input to the device for recording or feed-through.                                                   |
| MIC         | Microphone signal Input                                                                                                      |
| SP-         | Speaker(-): The negative Class D PWM provides a differential output with SP+ pin to directly drive an 8 Ω speaker            |
| SP+         | Speaker(+): The positive Class D PWM provides a differential output with the SP- pin to directly drive an 8 Ω speaker        |
| AUD/AUX     | Auxiliary Output: Depending upon the D7 of APC register, this output is either an AUD or AUX output.                         |
|             | AUD is a single-ended current output, whereas AUX is a single-ended voltage output.                                          |
| GND         | Ground                                                                                                                       |
| VCC         | 2.4V - 5.5V (5.0V Nominal)                                                                                                   |
| VOL         | Volume: This control has 8 levels of volume adjustment.                                                                      |
| FT          | Feed-through: In Standalone mode, when FT is engaged low, the AnaIn feed-through path is activated.                          |
| PLAY        | Playback: Pulsing PLAYto Low once initiates a playback operation.                                                            |
| REC         | Record: The device starts recording whenever REC switches from High to Low and stays at Low.                                 |
| ERASE       | Erase: When active, it starts an erase operation.                                                                            |
| FWD         | Forward: When triggered, it advances to the next message from the current location, when the device is in power-down status. |

---

## Test

-   [Tutorial I](https://bit.ly/3wQ9Qcj)
-   [Tutorial II](https://bit.ly/3uHuhq1)

-   [Tutorial Video I](https://www.youtube.com/watch?v=C13JUu38oZQ)
-   [Tutorial Video II](https://youtu.be/KDc2Z43DzT0)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [ISD1700 Datasheet](https://bit.ly/3sb73qy)
-   [ISD1700 Design Guide](https://bit.ly/2PSvQCI)
-   [ISD1700 Key description](https://bit.ly/Key-Description)

**to be updated..**

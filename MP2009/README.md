# MP3 Music Player Module - UART Control Serial, AVR/ARM/PIC

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The module is a kind of simple MP3 player device which is based on a high-quality MP3 audio
chip---YX5300. It can support 8k Hz ~ 48k Hz sampling frequency MP3 and WAV file formats.
There is a TF card socket on board, so you can plug the micro SD card that stores audio files. MCU
can control the MP3 playback state by sending commands to the module via UART port, such as
switch songs, change the volume and play mode and so on. You can also debug the module via USB
to UART module. It is compatible with Arduino / AVR / ARM / PIC

---

## Features (Specifications)

| Features                                                                            |
| ----------------------------------------------------------------------------------- |
| Support sampling frequency (kHz): 8 / 11.025 / 12 /16 / 22.05 / 24 / 32 / 44.1 / 48 |
| High quality                                                                        |
| Support file format: MP3 / WAV                                                      |
| Support Micro SD card, Micro SDHC Card                                              |
| 30 class adjustable volume                                                          |
| UART TTL serial control playback mode, baud rate is 9600bps                         |
| Power supply can be 3.2 ~ 5.2VDC                                                    |
| Control logic interface can be 3.3V / 5V TTL                                        |
| Compatible with Arduino UNO / Leonardo / Mega2560 / DUE                             |

### Specification

| Item                | Min | Typical                                     | Max | Unit |
| ------------------- | --- | ------------------------------------------- | --- | ---- |
| Power Supply(VCC)   | 3.2 | 5                                           | 5.2 | VDC  |
| Current(@VCC=5V)    |     |                                             | 200 | mA   |
| Logic interface     |     | 3.3V / 5V TTL                               |     |      |
| Supported Card Type |     | Micro SD card(<=2G); Mirco SDHC card(<=32G) |     |      |
| File system format  |     | Fat16 / Fat32 /                             |     |      |
| Uart baud rate      |     | 9600                                        |     | bps  |
| Dimensions          |     | 49 X 24 X 8.5                               |     | mm   |
| Net Weight          |     | 5                                           |     | g    |

---

## Pins

| Module | Arduino                           |
| ------ | --------------------------------- |
| VCC    | The positive 3.3-5 v power supply |
| GND    | Connect power negative            |
| RX     | D1 (TX)                           |
| TX     | D0 (RX)                           |

---

## Test

-   [Tutorial](https://www.hackster.io/javier-munoz-saez/arduino-mp3-player-catalex-2effef)

-   [Tutorial Video I](https://youtu.be/D9rsBf1b3CM)
-   [Tutorial Video II](https://youtu.be/-NfLxryxWZM)
-   [Tutorial Video III](https://youtu.be/HSLKefx1VK4)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [Datasheet](https://bit.ly/3dgDjn5)

-   **to be updated..**

# ISD1820 Voice Recording Recorder Module With Mic Sound

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

Voice Record Module is base on ISD1820, which a multiple‐message record/playback device.It can offers true single‐chip voice recording, no‐volatile storage, and playback capability around 10 seconds. This module is easy to use which you could direct control by push button on board or by Microcontroller such as Arduino, STM32, ChipKit etc. From these, you can easy control record , playback and repeat and so on.
It doesn't support to save multi recording. Next recording should be overwriting to the before recording.

---

## Features (Specifications)

| Features (Specifications)                                                             |
| ------------------------------------------------------------------------------------- |
| Operating Voltage: Wide power supply ranges from 2.4V to 5.5V DC                      |
| With the internal audio amplifier, this board can drive 8 Ohm 0.5W speakers directly. |
| An on-board microphone.                                                               |
| Dual operating modes                                                                  |
| Standalone mode                                                                       |
| Microcontroller Driven mode                                                           |
| Push‐button interface, playback can be edge or level activated                        |
| Record up to 20 seconds of audio                                                      |
| Automatic power-down mode (standby mode)                                              |
| Dimensions (LxWxH) in cm 8 x 6 x 3                                                    |

---

## Pins

![alt text](https://bit.ly/3fjnhew)

| Pin Number          | Description                                                                        |
| ------------------- | ---------------------------------------------------------------------------------- |
| VCC                 | DC 2.4-5.5V                                                                        |
| GND                 | Ground                                                                             |
| FT                  | FeedThrough This mode enables the Microphone to drive the speaker directly.        |
| REC/REC (Button)    | The REC input is an active‐HIGH record signal.                                     |
|                     | The module starts recording whenever REC is HIGH.                                  |
|                     | This pin must remain HIGH for the duration of the recording.                       |
|                     | REC takes precedence over either playback (PLAYLorPLAYE) signal.                   |
| P-E/PLAY-E (Button) | Playback, Edge‐activated: When a HIGH‐going transition is detected continues       |
|                     | until an End‐of‐Message (EOM) marker is encountered                                |
|                     | or the end of the memory space is reached.                                         |
| P-L/PLAY-L (Button) | Playback, Level‐activated, when this input pin level transits for LOW to HIGH,     |
|                     | a playback cycle is initiated.                                                     |
| SPI                 | The SP+‐ pins provide a direct drive for loudspeakers with impedances as low as8Ω. |
|                     | Note: This is not Serial Parallel Interface Pins.                                  |
| MIC                 | Microphone In:                                                                     |
|                     | the microphone input transfers its signals to the on‐chip pre-amplifier.           |

---

## Test

-   [Tutorial I](https://www.instructables.com/HOW-TO-USE-ISD1820-VOICE-RECORDER-AND-PLAYER/)
-   [Tutorial II](https://www.electronicshub.org/interfacing-isd1820-voice-recorder-module-with-arduino/)
-   [Tutorial III](https://robojax.com/learn/arduino/?vid=robojax-ISD1890-SoundRecorder)

-   [Tutorial Video I](https://youtu.be/wuyJwMVzeiA)
-   [Tutorial Video II](https://www.youtube.com/watch?v=10i74agujq8)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [ISD1820 Manual](https://bit.ly/3u0SmYO)
-   [For more information](https://components101.com/modules/isd1820-record-and-playback-module)

**to be updated..**

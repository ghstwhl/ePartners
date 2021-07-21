# Arduino Leonardo R3 ATmega32u4 Development Board

## Table of Contents

-   [Features](#features)
-   [Description](#description)
-   [Schematic](#schematic)
-   [Tutorials](#tutorials)
    -   [Test Environment](#test-environment)
        -   [Hardware](#hardware)
        -   [Software](#software)
    -   [Test](#test)
        -   [Test Code](#test-code)
        -   [Test Result](#test-result)
-   [References](#references)

---


## Description

The Leonardo differs from all preceding boards in that the ATmega32u4 has built-in USB communication, eliminating the need for a secondary processor.
This allows the Leonardo to appear to a connected computer as a mouse and keyboard, in addition to a virtual (CDC) serial / COM port.
It also has other implications for the behavior of the board.

---

## Features

| Features                   |                                                     |
| -------------------------- | --------------------------------------------------- |
| Microcontroller            | ATmega32u4                                          |
| Operationg Volatage        | 5V                                                  |
| Input Voltage(recommended) | 7-12V                                               |
| Digital I/O Pins           | 20 pins                                             |
| PWM Channels               | 7 pins                                              |
| Analog Pins                | 12 pins                                             |
| DC Current per I/O Pin     | 40mA                                                |
| DC Current per 3.3V Pin    | 50mA                                                |
| Flash Memory               | 32 KB (ATmega32u4) of which 4 KB used by bootloader |
| SRAM                       | 2.5 KB (ATmega32u4)                                 |
| EEPROM                     | 1 KB (ATmega32u4)                                   |
| Clock Speed                | 16 MHz                                              |
| LED_BUILTIN                | Digital pin 13                                      |
| Length                     | 68.6 mm                                             |
| Width                      | 53.3 mm                                             |
| Weight                     | 20g                                                 |
| USB Connector              | Type Micro B                                        |
| Power Jack                 | AC-to-DC adaptor                                    |
| ICSP Header                | 6 pins                                              |
| Reset Button               | tact button (Red)                                   |

---

## Tutorials

- [Intro](https://www.arduino.cc/en/Main/Arduino_BoardLeonardo)
- [Getting Started](https://www.arduino.cc/en/Guide/ArduinoLeonardoMicro)
- [Beginner Tutorial from scratch](https://tutorial.cytron.io/2012/11/23/getting-started-arduino-leonardo/)
- [Leonardo Keyboard Tutorial](https://www.youtube.com/watch?v=0fjuJOkk8y4)
- [Advanced Project](https://www.youtube.com/watch?v=A5s_9UNFDck)

For more tutorials and projects, please see [here](https://randomnerdtutorials.com/projects-arduino/)

---

## Troubleshooting

If the connection is disconnected while you upload the code, please check the power voltage on the board.

The USB cable has better connect to the PC or power supply directly.

---

## References

-   [Datasheet ATMEGA32U4](http://bit.ly/atmega32u4-datasheet)
-   [Arduino on Visual Studio code](https://maker.pro/arduino/tutorial/how-to-use-visual-studio-code-for-arduino)

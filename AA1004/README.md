# Arduino Leonardo R3 ATmega32u4 Development Board

## Table of Contents

-   [Features](#features)
-   [Description](#description)
-   [Schematic](#schematic)
-   [Test Environment](#test-environment)
    -   [Hardware](#hardware)
    -   [Software](#software)
-   [Test](#test)
    -   [Test Code](#test-code)
    -   [Test Result](#test-result)
-   [References](#references)

---

## Features

| Features                   |                                                     |
| -------------------------- | --------------------------------------------------- |
| Microcontroller            | ATmega32u4                                          |
| Operationg Volatage        | 5V                                                  |
| Input Voltage(recommended) | 7-12V                                               |
| Digital I/O Pins           | 20 pins                                             |
| PWM Channels               | 7 pins                                              |
| Analog Input Channels      | 12 pins                                             |
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
| USB Connector              | Type Micro                                          |
| Power Jack                 | AC-to-DC adaptor                                    |
| ICSP Header                | 6 pins                                              |
| Reset Button               | tact button (Red)                                   |

---

## Description

The Leonardo differs from all preceding boards in that the ATmega32u4 has built-in USB communication, eliminating the need for a secondary processor.
This allows the Leonardo to appear to a connected computer as a mouse and keyboard, in addition to a virtual (CDC) serial / COM port.
It also has other implications for the behavior of the board.

---

## Schematic

| ![alt text](assets/arduino-leonardo-schematic.png 'Leonardo Schematic') |
| ----------------------------------------------------------------------- |

---

## Test Environment

### Hardware

| ![alt text](http://bit.ly/aa1004-schematic 'Leonardo') |
| ------------------------------------------------------ |

### Software

| ![alt text](http://bit.ly/ep_software_1 'Leonardo') |
| --------------------------------------------------- |
| Go to Arduino [Home](https://www.arduino.cc/)       |

| ![alt text](http://bit.ly/ep_software_2 'Leonardo') |
| --------------------------------------------------- |
| Choose a appropriate file for your OS               |

| ![alt text](http://bit.ly/ep_software_3 'Leonardo')                       |
| ------------------------------------------------------------------------- |
| You can just download the file or contribute & download if you would like |

| ![alt text](http://bit.ly/ep_software_4 'Leonardo') |
| --------------------------------------------------- |
| Run the downloaded file                             |

| ![alt text](http://bit.ly/ep_software_5 'Leonardo') |
| --------------------------------------------------- |

| ![alt text](http://bit.ly/ep_software_6 'Leonardo') |
| --------------------------------------------------- |

| ![alt text](http://bit.ly/ep_software_7 'Leonardo') |
| --------------------------------------------------- |

| ![alt text](http://bit.ly/ep_software_8 'Leonardo') |
| --------------------------------------------------- |

| ![alt text](http://bit.ly/ep_software_9 'Leonardo') |
| --------------------------------------------------- |
| Click the 'close' button to complete                |

---

## Test

| ![alt text](https://bit.ly/ep_software_10 'Leonardo') |
| ----------------------------------------------------- |
| Run the Arduino IDE                                   |

| ![alt text](http://bit.ly/ep_software_11 'Leonardo') |
| ---------------------------------------------------- |
| Default page                                         |

| ![alt text](http://bit.ly/ep_software_12 'Leonardo') |
| ---------------------------------------------------- |
| Choose a blink example                               |

| ![alt text](http://bit.ly/aa1004-board 'Leonardo')                                        |
| ----------------------------------------------------------------------------------------- |
| Choose the "Arduino Uno" Board type & Port, if not selected                               |
| If the 'Port' button is unactivated, See the [Troubleshooting](#troubleshooting) section. |

| ![alt text](http://bit.ly/uno-upload 'Leonardo')                    |
| ------------------------------------------------------------------- |
| Click the 'upload' button. Compile will be processed automatically. |

| ![alt text](http://bit.ly/upload-done 'Leonardo') |
| ------------------------------------------------- |
| Check the 'Done uploading' message.               |

### Test Code

```c++
// the setup function runs once when you press reset or power the board
void setup() {
  // initialize digital pin LED_BUILTIN as an output.
  pinMode(LED_BUILTIN, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(1000);                       // wait for a second
  digitalWrite(LED_BUILTIN, LOW);    // turn the LED off by making the voltage LOW
  delay(1000);                       // wait for a second
}
```

### Test Result

| ![alt text](test/AA1004_blink.gif 'Leonardo') |
| --------------------------------------------- |
| Plese see the LED with 'L' sign on the board  |

---

## References

-   [Getting Started](https://www.arduino.cc/en/Guide/ArduinoLeonardoMicro)
-   [Datasheet ATMEGA32U4](http://bit.ly/atmega32u4-datasheet)
-   [Arduino on Visual Studio code](https://maker.pro/arduino/tutorial/how-to-use-visual-studio-code-for-arduino)

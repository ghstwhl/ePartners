# Arduino UNO R3 ATMEGA 328P (ATMEGA16U2 driver) Board (MAC, Windows, Linux)

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

| Features                   |                                                       |
| -------------------------- | ----------------------------------------------------- |
| Microcontroller            | ATmega328P                                            |
| USB Driver                 | ATMEGA16U2                                            |
| Operationg Volatage        | 5V                                                    |
| Input Voltage(recommended) | 7-12V                                                 |
| Digital I/O Pins           | 14 pins(of which 6 provide PWM output)                |
| PWM Channels               | 6 pins                                                |
| Analog Input Channels      | 6 pins                                                |
| DC Current per I/O Pin     | 20mA                                                  |
| DC Current per 3.3V Pin    | 50mA                                                  |
| Flash Memory               | 32 KB (ATmega328P) of which 0.5 KB used by bootloader |
| SRAM                       | 2 KB (ATmega328P)                                     |
| EEPROM                     | 1 KB (ATmega328P)                                     |
| Clock Speed                | 16 MHz                                                |
| LED_BUILTIN                | Digital pin 13                                        |
| Length                     | 68.6 mm                                               |
| Width                      | 53.4 mm                                               |
| Weight                     | 25g                                                   |
| USB Connector              | Type B                                                |
| Power Jack                 | AC-to-DC adaptor                                      |
| ICSP Header                | 6 pins                                                |
| Reset Button               | tact button (Red)                                     |

---

## Description

This Arduino Uno is a microcontroller board based on the ATMEGA 328P & ATMEGA 16U2 Driver.
It contains everything needed to support the microcontroller; simply connect it to a computer with a USB cable or power it with an AC-to-DC adapter or battery to get started.
The Uno differs from all preceding boards in that it does not use the FTDI USB-to-serial driver chip. Instead, it features the ATMEGA 16U2 programmed as a USB-to-serial converter.

---

## Schematic

| ![alt text](http://bit.ly/aa1009-schematic 'Leonardo Schematic') |
| ---------------------------------------------------------------- |

---

## Test Environment

### Hardware

| ![alt text](http://bit.ly/aa1009-uno 'Leonardo') |
| ------------------------------------------------ |

### Software

| ![alt text](http://bit.ly/ep_software_1 'Uno R3') |
| ------------------------------------------------- |
| Go to Arduino [Home](https://www.arduino.cc/)     |

| ![alt text](http://bit.ly/ep_software_2 'Uno R3') |
| ------------------------------------------------- |
| Choose a appropriate file for your OS             |

| ![alt text](http://bit.ly/ep_software_3 'Uno R3')                         |
| ------------------------------------------------------------------------- |
| You can just download the file or contribute & download if you would like |

| ![alt text](http://bit.ly/ep_software_4 'Uno R3') |
| ------------------------------------------------- |
| Run the downloaded file                           |

| ![alt text](http://bit.ly/ep_software_5 'Uno R3') |
| ------------------------------------------------- |

| ![alt text](http://bit.ly/ep_software_6 'Uno R3') |
| ------------------------------------------------- |

| ![alt text](http://bit.ly/ep_software_7 'Uno R3') |
| ------------------------------------------------- |

| ![alt text](http://bit.ly/ep_software_8 'Uno R3') |
| ------------------------------------------------- |

| ![alt text](http://bit.ly/ep_software_9 'Uno R3') |
| ------------------------------------------------- |
| Click the 'close' button to complete              |

---

## Test

| ![alt text](https://bit.ly/ep_software_10 'Uno R3') |
| --------------------------------------------------- |
| Run the Arduino IDE                                 |

| ![alt text](http://bit.ly/ep_software_11 'Uno R3') |
| -------------------------------------------------- |
| Default page                                       |

| ![alt text](http://bit.ly/ep_software_12 'Uno R3') |
| -------------------------------------------------- |
| Choose a blink example                             |

| ![alt text](http://bit.ly/aa1009-board 'Uno R3')                                          |
| ----------------------------------------------------------------------------------------- |
| Choose the "Arduino Uno" Board type & Port, if not selected                               |
| If the 'Port' button is unactivated, See the [Troubleshooting](#troubleshooting) section. |

| ![alt text](http://bit.ly/uno-upload 'Uno R3')                      |
| ------------------------------------------------------------------- |
| Click the 'upload' button. Compile will be processed automatically. |

| ![alt text](http://bit.ly/upload-done 'Uno R3') |
| ----------------------------------------------- |
| Check the 'Done uploading' message.             |

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

| ![alt text](test/AA1009_blink.gif 'Uno R3')  |
| -------------------------------------------- |
| Plese see the LED with 'L' sign on the board |

---

## References

-   [Getting Started](https://www.arduino.cc/en/Guide/ArduinoLeonardoMicro)
-   [Datasheet ATMEGA328P](http://bit.ly/atmega-328p)
-   [Datasheet ATMEGA16U2](http://bit.ly/atmega16u2-32u2_datasheet)
-   [Arduino on Visual Studio code](https://maker.pro/arduino/tutorial/how-to-use-visual-studio-code-for-arduino)

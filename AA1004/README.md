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
-   [Troubleshooting for Windows](#troubleshooting-for-windows)
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
| Length                     | 68.6 mm                                             |
| Width                      | 53.3 mm                                             |
| Weight                     | 20g                                                 |
| USB Connector              | Type B                                              |
| Power Jack                 | AC-to-DC adaptor                                    |
| ICSP Header                | 6 pins                                              |
| Reset Button               | tact button (Red)                                   |

---

## Description

-   It's 100% compatible with the same functionality
-   CH340G replace the Atmega16U2(USB Chip), faster and cheaper.

---

## Schematic

| ![alt text](assets/arduino-leonardo-schematic.png 'Leonardo Schematic') |
| ----------------------------------------------------------------------- |

---

## Test Environment

### Hardware

| ![alt text](assets/arduino_mega.png 'Leonardo') |
| ----------------------------------------------- |

### Software

| ![alt text](assets/software_1.png 'Leonardo') |
| --------------------------------------------- |
| Go to Arduino [Home](https://www.arduino.cc/) |

| ![alt text](assets/software_2.png 'Leonardo') |
| --------------------------------------------- |
| Choose a appropriate file for your OS         |

| ![alt text](assets/software_3.png 'Leonardo')                             |
| ------------------------------------------------------------------------- |
| You can just download the file or contribute & download if you would like |

| ![alt text](assets/software_4.png 'Leonardo') |
| --------------------------------------------- |
| Run the downloaded file                       |

| ![alt text](assets/software_5.png 'Leonardo') |
| --------------------------------------------- |

| ![alt text](assets/software_6.png 'Leonardo') |
| --------------------------------------------- |

| ![alt text](assets/software_7.png 'Leonardo') |
| --------------------------------------------- |

| ![alt text](assets/software_8.png 'Leonardo') |
| --------------------------------------------- |

| ![alt text](assets/software_9.png 'Leonardo') |
| --------------------------------------------- |

---

## Test

| ![alt text](assets/software_10.png 'Leonardo') |
| ---------------------------------------------- |
| Run the Arduino IDE                            |

| ![alt text](assets/software_11.png 'Leonardo') |
| ---------------------------------------------- |
| Default page                                   |

| ![alt text](assets/software_12.png 'Leonardo') |
| ---------------------------------------------- |
| Choose a blink example                         |

| ![alt text](assets/software_13.png 'Leonardo')                                            |
| ----------------------------------------------------------------------------------------- |
| Choose the "Arduino Uno" Board type & Port, if not selected                               |
| If the 'Port' button is unactivated, See the [Troubleshooting](#troubleshooting) section. |

| ![alt text](assets/software_14.png 'Leonardo')                      |
| ------------------------------------------------------------------- |
| Click the 'upload' button. Compile will be processed automatically. |

| ![alt text](assets/software_15.png 'Leonardo') |
| ---------------------------------------------- |
| Check the 'Done uploading' message.            |

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

| ![alt text](assets/arduino_mega_blink.gif 'Leonardo') |
| ----------------------------------------------------- |

---

## Troubleshooting for Windows

| ![alt text](assets/trouble_1.png 'Port blocked')                                            |
| ------------------------------------------------------------------------------------------- |
| If the 'port' button is unactivated, you need to install the CH340 Driver [here.](Drivers/) |
| For more information, please visit [here.](https://sparks.gogo.co.nz/ch340.html)            |

| ![alt text](assets/trouble_2.png 'Port blocked') |
| ------------------------------------------------ |
| After downloading, Extract the Zip file          |

| ![alt text](assets/trouble_3.png 'Port blocked') |
| ------------------------------------------------ |
| Click the 'Extract'                              |

| ![alt text](assets/trouble_4.png 'Port blocked')       |
| ------------------------------------------------------ |
| You will see an app, just run it to install the driver |

| ![alt text](assets/trouble_6.png 'Port blocked') |
| ------------------------------------------------ |
| Click the 'Install'                              |

| ![alt text](assets/trouble_7.png 'Port blocked')                                |
| ------------------------------------------------------------------------------- |
| Then you will see this message! Restart the Arduino IDE                         |
| If you fail to install, connect the Arduino to the PC and then retry to install |

---

## References

-   [Arduino Home](https://www.arduino.cc/)
-   [Datasheet](http://bit.ly/atmega16u4-32u4_datasheet)
-   [Arduino on Visual Studio code](https://maker.pro/arduino/tutorial/how-to-use-visual-studio-code-for-arduino)

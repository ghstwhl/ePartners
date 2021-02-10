# Arduino Mega2560 R3-16AU CH340G Development Board

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

| Features                   |                                          |
| -------------------------- | ---------------------------------------- |
| Microcontroller            | ATmega2560                               |
| Operationg Volatage        | 5V                                       |
| Input Voltage(recommended) | 7-12V                                    |
| Digital I/O Pins           | 54 pins (of which 15 provide PWM output) |
| Analog Input Pins          | 16 pins                                  |
| DC Current per I/O Pin     | 20mA                                     |
| DC Current per 3.3V Pin    | 50mA                                     |
| Flash Memory               | 256 KB of which 8 KB used by bootloader  |
| SRAM                       | 8 KB                                     |
| EEPROM                     | 4 KB                                     |
| Clock Speed                | 16 MHz (ceramic resonator)               |
| LED_BUILTIN                | Digital pin 13                           |
| Length                     | 101.52 mm                                |
| Width                      | 53.3 mm                                  |
| Weight                     | 37g                                      |
| USB Connector              | Type B                                   |
| Power Jack                 | AC-to-DC adaptor                         |
| ISCP Header                | 6 pins                                   |
| Reset Button               | tact button (Red)                        |

---

## Description

-   It's 100% compatible with the same functionality
-   CH340G replace the Atmega16U2(USB Chip), faster and cheaper.

---

## Schematic

| ![alt text](assets/Arduino-mega2560_R3-schematic.png 'Mega Schematic') |
| ---------------------------------------------------------------------- |

---

## Test Environment

### Hardware

| ![alt text](assets/arduino_uno.png 'Uno R3') |
| -------------------------------------------- |

### Software

| ![alt text](assets/software_1.png 'Uno R3')   |
| --------------------------------------------- |
| Go to Arduino [Home](https://www.arduino.cc/) |

| ![alt text](assets/software_2.png 'Uno R3') |
| ------------------------------------------- |
| Choose a appropriate file for your OS       |

| ![alt text](assets/software_3.png 'Uno R3')                               |
| ------------------------------------------------------------------------- |
| You can just download the file or contribute & download if you would like |

| ![alt text](assets/software_4.png 'Uno R3') |
| ------------------------------------------- |
| Run the downloaded file                     |

| ![alt text](assets/software_5.png 'Uno R3') |
| ------------------------------------------- |

| ![alt text](assets/software_6.png 'Uno R3') |
| ------------------------------------------- |

| ![alt text](assets/software_7.png 'Uno R3') |
| ------------------------------------------- |

| ![alt text](assets/software_8.png 'Uno R3') |
| ------------------------------------------- |

| ![alt text](assets/software_9.png 'Uno R3') |
| ------------------------------------------- |

---

## Test

| ![alt text](assets/software_10.png 'Uno R3') |
| -------------------------------------------- |
| Run the Arduino IDE                          |

| ![alt text](assets/software_11.png 'Uno R3') |
| -------------------------------------------- |
| Default page                                 |

| ![alt text](assets/software_12.png 'Uno R3') |
| -------------------------------------------- |
| Choose a blink example                       |

| ![alt text](assets/software_13.png 'Uno R3')                                              |
| ----------------------------------------------------------------------------------------- |
| Choose the "Arduino Uno" Board type & Port, if not selected                               |
| If the 'Port' button is unactivated, See the [Troubleshooting](#troubleshooting) section. |

| ![alt text](assets/software_14.png 'Uno R3')                        |
| ------------------------------------------------------------------- |
| Click the 'upload' button. Compile will be processed automatically. |

| ![alt text](assets/software_15.png 'Uno R3') |
| -------------------------------------------- |
| Check the 'Done uploading' message.          |

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

| ![alt text](assets/Arduino_Uno.gif 'Uno R3') |
| -------------------------------------------- |

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
-   [Data Sheet](http://ww1.microchip.com/downloads/en/devicedoc/atmel-2549-8-bit-avr-microcontroller-atmega640-1280-1281-2560-2561_datasheet.pdf)
-   [Arduino on VScode](https://maker.pro/arduino/tutorial/how-to-use-visual-studio-code-for-arduino)
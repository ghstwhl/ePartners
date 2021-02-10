# Arduino UNO R3 MEGA328P CH340 Development Board

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

| Features                   |                                                       |
| -------------------------- | ----------------------------------------------------- |
| Microcontroller            | ATmega328P                                            |
| Operationg Volatage        | 5V                                                    |
| Input Voltage(recommended) | 7-12V                                                 |
| Digital I/O Pins           | 14 pins (of which 6 provide PWM output)               |
| Analog Input Pins          | 6 pins                                                |
| DC Current per I/O Pin     | 40mA                                                  |
| DC Current per 3.3V Pin    | 50mA                                                  |
| Flash Memory               | 32 KB (ATmega328P) of which 0.5 KB used by bootloader |
| SRAM                       | 2 KB (ATmega328P)                                     |
| EEPROM                     | 1 KB (ATmega328P)                                     |
| Clock Speed                | 16 MHz (ceramic resonator)                            |
| Length                     | 68.66 mm                                              |
| Width                      | 53.4 mm                                               |
| Weight                     | 25g                                                   |
| USB Connector              | Type B                                                |
| Power Jack                 | AC-to-DC adaptor                                      |
| ISCP Header                | 6 pins                                                |
| Reset Button               | Red one                                               |

---

## Description

-   This Arduino Uno is a microcontroller board based on the CH340.
-   It contains everything needed to support the microcontroller; simply connect it to a computer with a USB cable or power it with an AC-to-DC adapter or battery to get started.
-   The Uno differs from all preceding boards in that it does not use the FTDI USB-to-serial driver chip. Instead, it features the CH340 programmed as a USB-to-serial converter

---

## Schematic

| ![alt text](assets/arduino_uno_schematic_ch340.png 'Uno Schematic') |
| ------------------------------------------------------------------- |

---

## Test Environment

### Hardware

| ![alt text](assets/arduino_uno.png 'Uno R3') |
| -------------------------------------------- |

### Software

| ![alt text](assets/software_1.png 'Uno R3') |
| ------------------------------------------- |

| Go to Arduino [Home](https://www.arduino.cc/)

| ![alt text](assets/software_2.png 'Uno R3') |
| ------------------------------------------- |

| ![alt text](assets/software_3.png 'Uno R3') |
| ------------------------------------------- |

| ![alt text](assets/software_4.png 'Uno R3') |
| ------------------------------------------- |

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
-   [Arduino on VScode](https://maker.pro/arduino/tutorial/how-to-use-visual-studio-code-for-arduino)

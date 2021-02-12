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

| ![alt text](assets/arduino-leonardo.png 'Leonardo') |
| --------------------------------------------------- |

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

| ![alt text](assets/software_13.png 'Leonardo')              |
| ----------------------------------------------------------- |
| Choose the "Arduino Uno" Board type & Port, if not selected |

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

| ![alt text](assets/arduino_leonardo_blink.gif 'Leonardo') |
| --------------------------------------------------------- |

---

## References

-   [Getting Started](https://www.arduino.cc/en/Guide/ArduinoLeonardoMicro)
-   [Datasheet](http://bit.ly/atmega16u4-32u4_datasheet)
-   [Arduino on Visual Studio code](https://maker.pro/arduino/tutorial/how-to-use-visual-studio-code-for-arduino)

| ![alt text](https://lh3.googleusercontent.com/O46-8glyh3iiiPEyJqj25KvNWSmrzv7LQjBvVj_YRbBNoXmmS20TGmHBGqMzVeaRvIQnmn-0EqTIqqEi1pxYa0_ZPeRfVJ9r2QlEwcPcZTZoJXAhCBP6KMESnvlyM-z4ZgfrWQzZpcfrPwu_srq0kxssquz-zeinlRCMLlqjx2sxcxnn7oKVlVJ3bnLRbYMePbatXEdwM6ybT4cv_pO6iHcFwitQZcVKovJOFgH9Hnx3WlYuaWSMcnouwXFpqZYF4u7U7-lwi9MfJ6Vg-F9g1CzKiRnfRN40daPrL7ZgJ412EZNtfl0VwoTZzaH4SvFM-sx8RqnuS1izMXzafhIyPVpfhdw-Fk-fIds3Bkl1OU4umXyVKRSbuLJpafrY5npXE0L5keGhc9bxKWAlXlrQvVmaBdr3qbr-22taRtKcryTe6V1sqJZk4POd9pgxkaftaUlFK4EdVnGloVPME0x4DDeG-Kzos2npc2oIHuFua_RTzLDyim-qbJ4VF4CCq6J1DNB_lQphmuyqO6fn7GMWnUoG_KUpsJfuNtDoOrIy5qxto2TzSBgfhP--MeMQGJ48HZAtbpO8XlVSJb0aWD7EWkniEf9QLh3F0c4EgUiQlkYJXZ8EfONWYDy2oiihaFKPefdXFb51ftP5qS7F2_GV77OMfogX5kNwxU_kEqK_WaZKj1Nr9681fNgZ9eK0XQ=w300-h226-no?authuser=0 'leo') |

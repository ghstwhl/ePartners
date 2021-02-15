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
| Clock Speed                | 16 MHz                                   |
| LED_BUILTIN                | Digital pin 13                           |
| Length                     | 101.52 mm                                |
| Width                      | 53.3 mm                                  |
| Weight                     | 37g                                      |
| USB Connector              | Type B                                   |
| Power Jack                 | AC-to-DC adaptor                         |
| ICSP Header                | 6 pins                                   |
| Reset Button               | tact button (Red)                        |

---

## Description

It's 100% compatible with the same functionality
CH340G replace the Atmega16U2(USB Chip), faster and cheaper.
The Mega 2560 board is compatible with most shields designed for the Uno and the former boards Duemilanove or Diecimila.

---

## Schematic

| ![alt text](http://bit.ly/aa1002-schematic 'Mega Schematic') |
| ------------------------------------------------------------ |

---

## Test Environment

### Hardware

| ![alt text](http://bit.ly/aa1002-mega 'Mega2560 R3') |
| ---------------------------------------------------- |

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

| ![alt text](http://bit.ly/aa1002-board 'Uno R3')                                          |
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

| ![alt text](test/AA1002_blink.gif 'Mega2560 R3') |
| ------------------------------------------------ |

---

## Troubleshooting for Windows

| ![alt text](http://bit.ly/trouble-1 'Port blocked')                                         |
| ------------------------------------------------------------------------------------------- |
| If the 'port' button is unactivated, you need to install the CH340 Driver [here.](Drivers/) |
| For more information, please visit [here.](https://sparks.gogo.co.nz/ch340.html)            |

| ![alt text](http://bit.ly/trouble-2 'Port blocked') |
| --------------------------------------------------- |
| After downloading, Extract the Zip file             |

| ![alt text](http://bit.ly/trouble-3 'Port blocked') |
| --------------------------------------------------- |
| Click the 'Extract'                                 |

| ![alt text](http://bit.ly/trouble-4 'Port blocked')    |
| ------------------------------------------------------ |
| You will see an app, just run it to install the driver |

| ![alt text](http://bit.ly/trouble-5 'Port blocked') |
| --------------------------------------------------- |
| Click the 'Install'                                 |

| ![alt text](http://bit.ly/trouble-6 'Port blocked')                             |
| ------------------------------------------------------------------------------- |
| Then you will see this message! Restart the Arduino IDE                         |
| If you fail to install, connect the Arduino to the PC and then retry to install |

---

## References

-   [Getting Started](https://www.arduino.cc/en/Guide/ArduinoMega2560)
-   [Datasheet](http://bit.ly/Arduino-Mega2560-datasheet)
-   [Arduino on Visual Studio code](https://maker.pro/arduino/tutorial/how-to-use-visual-studio-code-for-arduino)

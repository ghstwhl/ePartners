# Arduino Nano V3.0 ATmega328P Controller(CH340G Driver) Development Board

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
| Microcontroller            | ATmega328P                                          |
| USB Driver                 | CH340G                                              |
| Operationg Volatage        | 5V                                                  |
| Input Voltage(recommended) | 7-12V                                               |
| Digital I/O Pins           | 14 pins (TX, RX, D2~D13)                            |
| PWM Channels               | 6 pins (D3, D5, D6, D9, D10, D11)                   |
| Analog Input Channels      | 2 pins (A0~A7)                                      |
| DC Current per I/O Pin     | 40mA                                                |
| Flash Memory               | 32 KB (ATmega328P) of which 2 KB used by bootloader |
| SRAM                       | 2 KB                                                |
| EEPROM                     | 1 KB                                                |
| Clock Speed                | 16 MHz                                              |
| LED_BUILTIN                | Digital pin 13                                      |
| Length                     | 45 mm                                               |
| Width                      | 18 mm                                               |
| Weight                     | 7g                                                  |
| USB Connector              | Type Mini-B                                         |
| ICSP Header                | 6 pins                                              |
| Reset Button               | tact button (White)                                 |

---

## Description

The Arduino Nano is a small, complete, and breadboard-friendly board based on the ATmega328 (Arduino Nano 3.x). It has more or less the same functionality of the Arduino Duemilanove, but in a different package. It lacks only a DC power jack, and works with a Mini-B USB cable instead of a standard one.

---

## Schematic

| ![alt text](http://bit.ly/aa1011-schematic 'Nano Schematic') |
| ------------------------------------------------------------ |

---

## Test Environment

### Hardware

| ![alt text](http://bit.ly/aa1011 'Nano') |
| ---------------------------------------- |

### Software

| ![alt text](http://bit.ly/ep_software_1 'Nano') |
| ----------------------------------------------- |
| Go to Arduino [Home](https://www.arduino.cc/)   |

| ![alt text](http://bit.ly/ep_software_2 'Nano') |
| ----------------------------------------------- |
| Choose a appropriate file for your OS           |

| ![alt text](http://bit.ly/ep_software_3 'Nano')                           |
| ------------------------------------------------------------------------- |
| You can just download the file or contribute & download if you would like |

| ![alt text](http://bit.ly/ep_software_4 'Nano') |
| ----------------------------------------------- |
| Run the downloaded file                         |

| ![alt text](http://bit.ly/ep_software_5 'Nano') |
| ----------------------------------------------- |

| ![alt text](http://bit.ly/ep_software_6 'Nano') |
| ----------------------------------------------- |

| ![alt text](http://bit.ly/ep_software_7 'Nano') |
| ----------------------------------------------- |

| ![alt text](http://bit.ly/ep_software_8 'Nano') |
| ----------------------------------------------- |

| ![alt text](http://bit.ly/ep_software_9 'Nano') |
| ----------------------------------------------- |
| Click the 'close' button to complete            |

---

## Test

| ![alt text](https://bit.ly/ep_software_10 'Nano') |
| ------------------------------------------------- |
| Run the Arduino IDE                               |

| ![alt text](http://bit.ly/ep_software_11 'Nano') |
| ------------------------------------------------ |
| Default page                                     |

| ![alt text](http://bit.ly/ep_software_12 'Nano') |
| ------------------------------------------------ |
| Choose a blink example                           |

| ![alt text](http://bit.ly/aa1011-board 'Nano')                                            |
| ----------------------------------------------------------------------------------------- |
| Choose the "Arduino Uno" Board type & Port, if not selected                               |
| If the 'Port' button is unactivated, See the [Troubleshooting](#troubleshooting) section. |

| ![alt text](http://bit.ly/uno-upload 'Nano')                        |
| ------------------------------------------------------------------- |
| Click the 'upload' button. Compile will be processed automatically. |

| ![alt text](http://bit.ly/upload-done 'Nano') |
| --------------------------------------------- |
| Check the 'Done uploading' message.           |

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

| ![alt text](test/AA1011_blink.gif 'Nano')    |
| -------------------------------------------- |
| Plese see the LED with 'L' sign on the board |

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

-   [Getting Started](https://www.arduino.cc/en/Guide/ArduinoLeonardoMicro)
-   [Datasheet ATMEGA328P](http://bit.ly/atmega-328p)
-   [Datasheet CH340](http://bit.ly/ch340-datasheet)
-   [Arduino on Visual Studio code](https://maker.pro/arduino/tutorial/how-to-use-visual-studio-code-for-arduino)

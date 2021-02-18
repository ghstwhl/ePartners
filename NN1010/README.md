# Arduino Pro Micro ATmega32U4 Controller Development Board

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
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Features

| Features            |                         |
| ------------------- | ----------------------- |
| Microcontroller     | ATmega32u4              |
| Operationg Volatage | 5V                      |
| Digital I/O Pins    | 12 pins                 |
| PWM Channels        | 5 pins                  |
| 10 bits ADC pins    | 4 pins                  |
| Clock Speed         | 16 MHz                  |
| LED_BUILTIN         | RX, TX                  |
| Length              | 33 mm                   |
| Width               | 18 mm                   |
| USB Connector       | Type Micro B (On Board) |

---

## Description

This is a brief guide to getting started with the Pro Micro Arduino Board (Atmega32U4) - not to be confused with the Pro Mini (which utilises the Atmega328P)! Note that the Pro Micro board comes in two flavours/flavors - 5V @ 16 MHz and 3.3V @ 8 MHz, so make sure you know which you have before getting started. It should be indicated on the bottom silkscreen of the bottom, or you could take a voltmeter and measure VCC against GND - it will be either 5V or 3.3V.

---

## Schematic

| ![alt text](https://bit.ly/2Zeson6 'Pro micro Schematic') |
| --------------------------------------------------------- |

---

## Tutorials

### Test Environment

#### Hardware

| ![alt text](https://bit.ly/2Zv0ofj 'Pro Micro') |
| ----------------------------------------------- |
| Pro micro 5V/16MHz                              |

### Software

| ![alt text](http://bit.ly/ep_software_1 'Pro Micro') |
| ---------------------------------------------------- |
| Go to Arduino [Home](https://www.arduino.cc/)        |

| ![alt text](http://bit.ly/ep_software_2 'Pro Micro') |
| ---------------------------------------------------- |
| Choose a appropriate file for your OS                |

| ![alt text](http://bit.ly/ep_software_3 'Pro Micro')                      |
| ------------------------------------------------------------------------- |
| You can just download the file or contribute & download if you would like |

| ![alt text](http://bit.ly/ep_software_4 'Pro Micro') |
| ---------------------------------------------------- |
| Run the downloaded file                              |

| ![alt text](http://bit.ly/ep_software_5 'Pro Micro') | ![alt text](http://bit.ly/ep_software_6 'Pro Micro') |
| ---------------------------------------------------- | ---------------------------------------------------- |

| ![alt text](http://bit.ly/ep_software_7 'Pro Micro') | ![alt text](http://bit.ly/ep_software_8 'Pro Micro') |
| ---------------------------------------------------- | ---------------------------------------------------- |

| ![alt text](http://bit.ly/ep_software_9 'Pro Micro') |
| ---------------------------------------------------- |
| Click the 'close' button to complete                 |

---

### Test

#### Connection

| Pro Micro | FTDI Converter |
| --------- | -------------- |
| GND       | GND            |
| VCC       | VCC            |
| RX        | TX             |
| TX        | RX             |

#### Blink Test

| ![alt text](https://bit.ly/ep_software_10 'Pro Micro') |
| ------------------------------------------------------ |
| Run the Arduino IDE                                    |

| ![alt text](http://bit.ly/ep_software_11 'Pro Micro') |
| ----------------------------------------------------- |
| Default page                                          |

| ![alt text](http://bit.ly/ep_software_12 'Pro Micro') |
| ----------------------------------------------------- |
| Choose a blink example                                |

| ![alt text](https://bit.ly/2N65E6k 'Pro Micro')               |
| ------------------------------------------------------------- |
| Choose the "Arduino Micro" Board type & Port, if not selected |

| ![alt text](http://bit.ly/uno-upload 'Pro Micro')                   |
| ------------------------------------------------------------------- |
| Click the 'upload' button. Compile will be processed automatically. |

| ![alt text](http://bit.ly/upload-done 'Pro Micro') |
| -------------------------------------------------- |
| Check the 'Done uploading' message.                |

#### Test Code

```c++
int RXLED = 17; // The RX LED has a defined Arduino pin
int TXLED = 30; // The TX LED has a defined Arduino pin

// the setup function runs once when you press reset or power the board
void setup() {

  pinMode(RXLED, OUTPUT); // Set RX LED as an output
  pinMode(TXLED, OUTPUT); // Set TX LED as an output
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(RXLED, HIGH); // set the LED off
  digitalWrite(TXLED, LOW); // set the LED off
  delay(300);                       // wait for a second
  digitalWrite(RXLED, LOW); // set the LED on
  digitalWrite(TXLED, HIGH); // set the LED on
  delay(300);                       // wait for a second
}
```

#### Test Result

| ![alt text](test/NN1010_blink.gif 'Pro Micro') |
| ---------------------------------------------- |
| Plese see the LED with 'L' sign on the board   |

---

## Troubleshooting

If the connection is disconnected while you upload the code, please check the power voltage on the board.

The USB cable has better connect to the PC or power supply directly.

---

## References

-   [Getting Started](http://bit.ly/3deGI7l)
-   [Datasheet ATMEGA32U4](http://bit.ly/atmega32u4-datasheet)
-   [Arduino on Visual Studio code](https://maker.pro/arduino/tutorial/how-to-use-visual-studio-code-for-arduino)
-   [Tutorial](https://youtu.be/nxPgun6xjHM)

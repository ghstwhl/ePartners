# Arduino Pro Mini ATmega328/328P Controller Development Board

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
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Features

| Features                  |                                                |
| ------------------------- | ---------------------------------------------- |
| Microcontroller           | ATmega328P                                     |
| Board Power Supply        | 3.35 -12 V (3.3V model) or 5 - 12 V (5V model) |
| Circuit Operating Voltage | 3.3V or 5V (Depending on model)                |
| Digital I/O Pins          | 14 pins (TX, RX, D2~D13)                       |
| PWM Channels              | 6 pins (D3, D5, D6, D9, D10, D11)              |
| Analog Pins               | 8 pins (A0~A7), A6 & A7 (Analog Input only)    |
| External Interrupt        | 2                                              |
| DC Current per I/O Pin    | 40mA                                           |
| Flash Memory              | 32 KB of which 2 KB used by bootloader         |
| SRAM                      | 2 KB                                           |
| EEPROM                    | 1 KB                                           |
| Clock Speed               | 8 MHz(3.3V version), 16 MHz(5V version)        |
| LED_BUILTIN               | Digital pin 13                                 |
| UART                      | 1                                              |
| SPI                       | 1                                              |
| I2C                       | 1                                              |
| Reset Button              | tact button (White)                            |

---

## Description

This board was developed for applications and installations where space is premium and projects are made as permanent set ups. Small, available in 3.3 V and 5 V versions, powered by ATmega328/328P.

Atmega328P and Atmega328 are the same every sense architecturally. So you can just drop in a 328p in place of a 328 and vice versa.<br/>
Atmega328P just consumes lower power than Atmega328. Look up the numbers in the datasheet. This means that the 328P is manufactured in a finer process than the 328.<br/>
The chip signatures of 328P and 328 are different. So if any program is reading these signatures to make a decision (like avrdude in arduino), then you will have to watch out as the software could complain saying that the wrong chip was used.

---

## Schematic

| ![alt text](http://bit.ly/op2001-schematic 'Pro mini Schematic') |
| ---------------------------------------------------------------- |

---

## Test Environment

### Hardware

| ![alt text](https://bit.ly/3aiIthN 'Pro mini') | ![alt text](https://bit.ly/3qnKMFZ 'Pro mini') |
| ---------------------------------------------- | ---------------------------------------------- |
| Pro mini 5V                                    | Pro mini 3.3V                                  |

| ![alt text](https://bit.ly/2LQ30Rw 'USB to TTL Converter') |
| ---------------------------------------------------------- |
| FTDI USB to TTL Adapter                                    |

### Software

| ![alt text](http://bit.ly/ep_software_1 'Pro mini') |
| --------------------------------------------------- |
| Go to Arduino [Home](https://www.arduino.cc/)       |

| ![alt text](http://bit.ly/ep_software_2 'Pro mini') |
| --------------------------------------------------- |
| Choose a appropriate file for your OS               |

| ![alt text](http://bit.ly/ep_software_3 'Pro mini')                       |
| ------------------------------------------------------------------------- |
| You can just download the file or contribute & download if you would like |

| ![alt text](http://bit.ly/ep_software_4 'Pro mini') |
| --------------------------------------------------- |
| Run the downloaded file                             |

| ![alt text](http://bit.ly/ep_software_5 'Pro mini') | ![alt text](http://bit.ly/ep_software_6 'Pro mini') |
| --------------------------------------------------- | --------------------------------------------------- |

| ![alt text](http://bit.ly/ep_software_7 'Pro mini') | ![alt text](http://bit.ly/ep_software_8 'Pro mini') |
| --------------------------------------------------- | --------------------------------------------------- |

| ![alt text](http://bit.ly/ep_software_9 'Pro mini') |
| --------------------------------------------------- |
| Click the 'close' button to complete                |

---

## Test

### Connection

| Pro Mini | FTDI Adapter |
| -------- | ------------ |
| GND      | GND          |
| VCC      | VCC          |
| RX       | TX           |
| TX       | RX           |

| ![alt text](https://bit.ly/ep_software_10 'Pro mini') |
| ----------------------------------------------------- |
| Run the Arduino IDE                                   |

| ![alt text](http://bit.ly/ep_software_11 'Pro mini') |
| ---------------------------------------------------- |
| Default page                                         |

| ![alt text](http://bit.ly/ep_software_12 'Pro mini') |
| ---------------------------------------------------- |
| Choose a blink example                               |

| ![alt text](https://bit.ly/2NaoN73 'Pro mini')                          |
| ----------------------------------------------------------------------- |
| Choose the "Arduino Pro or Pro mini" Board type & Port, if not selected |
| If you use 3.3V, please change the "Processor" type to "3.3V, 8MHz"     |

| ![alt text](http://bit.ly/uno-upload 'Pro mini')                    |
| ------------------------------------------------------------------- |
| Click the 'upload' button. Compile will be processed automatically. |

| ![alt text](http://bit.ly/upload-done 'Pro mini') |
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

| ![alt text](test/OP2001_blink.gif 'Pro mini') |
| --------------------------------------------- |
| Plese see the LED with 'L' sign on the board  |

---

## Troubleshooting

| ![alt text](https://bit.ly/3am5Gjj 'Pro mini Troubleshoot')                                              |
| -------------------------------------------------------------------------------------------------------- |
| If you encounter the error while you upload the code or 'Uploading' doesn't proceed,                     |
| Please try uploading again and then press the 'reset' button as soon as you see the 'Uploading' message. |

---

## References

-   [Getting Started](https://www.arduino.cc/en/Guide/ArduinoLeonardoMicro)
-   [Datasheet ATMEGA328P](http://bit.ly/atmega-328p)
-   [Arduino on Visual Studio code](https://maker.pro/arduino/tutorial/how-to-use-visual-studio-code-for-arduino)

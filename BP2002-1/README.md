# ESP32 38P Development Board WiFi+Bluetooth Ultra-Low Power Consumption Dual Core

## Table of Contents

-   [Description](#description)
-   [Features](#features)
-   [Pinout](#pinout)
-   [Test-environment](#test-environment)
    -   [Hardware](#hardware)
    -   [Software](#software)
-   [Test](#test)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Description

ESP32 is a series of low-cost, low-power system on a chip microcontrollers with integrated Wi-Fi and dual-mode Bluetooth. The ESP32 series employs a Tensilica Xtensa LX6 microprocessor in both dual-core and single-core variations and includes built-in antenna switches, RF balun, power amplifier, low-noise receive amplifier, filters, and power-management modules. ESP32 is created and developed by Espressif Systems, a Shanghai-based Chinese company, and is manufactured by TSMC using their 40 nm process. It is a successor to the ESP8266 microcontroller.

## Features

| Features        | Details                                            |
| --------------- | -------------------------------------------------- |
| Architecture    | 32 bits                                            |
| Number of cores | 2(dual core)                                       |
| Memory          | 512KB SRAM                                         |
| Wi-Fi           | 2.4 GHz up to 150 Mbits/s                          |
| Bluetooth       | BLE (Bluetooth Low Energy) and legacy Bluetooth    |
| Pins            | 30 or 38 (depends on the model)                    |
| Peripherals     | ADC (analog to digital converter)                  |
|                 | DAC (digital to analog converter)                  |
|                 | I2C (Inter-Integrated Circuit)                     |
|                 | UART (universal asynchronous receiver/transmitter) |
|                 | SPI (Serial Peripheral Interface)                  |
|                 | I2S (Integrated Inter-IC Sound)                    |
|                 | CAN 2.0 (Controller Area Netwokr)                  |
|                 | Motor PWM (pulse width modulation)                 |
|                 | LED PWM (pulse width modulation)                   |
| Clock frequency | Up to 240 MHz                                      |
| Etc..           |                                                    |

## Pinout

![alt text](https://bit.ly/3eJg3QD 'pinout')

## Test Environment

### Hardware

![alt text](https://bit.ly/3tlr7aS 'ESP32-38p')

---

### Software

-   Windows version (If you use Mac or Linux, please see [here](http://bit.ly/3tmXwxF))
-   Arduino IDE [Latest version should be installed](https://www.arduino.cc/en/software)
-   ESP32 Add-on in Arduino IDE (Please see [here](http://bit.ly/2UnFLxy))
-   Add ESP32 board in Arduino IDE (Please see [here](http://bit.ly/3tmXwxF))

---

## Test

-   Open the following example under <b>File > Examples > WiFi(ESP32) > WiFiScan</b>

![alt text](https://bit.ly/2Ozqcoy 'example')

### Test Result

-   The result of test should be like below (result may differ)

![alt text](https://bit.ly/3ls1xyk 'result')

## Troubleshooting

-   If you encounter an error while uploading, please see the troubleshooting section [here](http://bit.ly/3tmXwxF)

---

## References

-   Tutorials

    -   [ESP32 Tutorials I](https://randomnerdtutorials.com/getting-started-with-esp32/)

    -   [ESP32 Tutorials II](https://randomnerdtutorials.com/installing-the-esp32-board-in-arduino-ide-windows-instructions/)

    -   [ESP32 Tutorials III](http://esp32.net/)

    -   [ESP32 Tutorials with Arduino](https://www.dfrobot.com/blog-964.html)

-   Data sheet
    -   [ESP32 series data sheet](https://www.mouser.com/datasheet/2/891/esp-wroom-32_datasheet_en-1223836.pdf)

to be updated..

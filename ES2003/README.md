# ESP32-CAM Tutorial

## Table of Contents

-   [Descriptions](#descriptions)
-   [features](#features)
-   [Connections](#connections)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The ESP32-CAM is a full-featured microcontroller that also has an integrated video camera and microSD card socket. It’s inexpensive and easy to use, and is perfect for IoT devices requiring a camera with advanced functions like image tracking and recognition.

---

## Features (Specifications)

| 802.11b/g/n Wi-Fi                              |
| ---------------------------------------------- |
| Bluetooth 4.2 with BLE                         |
| UART, SPI, I2C and PWM interfaces              |
| Clock speed up to 160 MHz                      |
| Computing power up to 600 DMIPS                |
| 520 KB SRAM plus 4 MB PSRAM                    |
| Supports WiFi Image Upload                     |
| Multiple Sleep modes                           |
| Firmware Over the Air (FOTA) upgrades possible |
| 9 GPIO ports                                   |
| Built-in Flash LED                             |

---

## Connections

-   [Pinout Diagram](https://randomnerdtutorials.com/esp32-cam-ai-thinker-pinout/)

| OV2640 CAMERA | ESP32   | Variable name in code |
| ------------- | ------- | --------------------- |
| D0            | GPIO 5  | Y2_GPIO_NUM           |
| D1            | GPIO 18 | Y3_GPIO_NUM           |
| D2            | GPIO 19 | Y4_GPIO_NUM           |
| D3            | GPIO 21 | Y5_GPIO_NUM           |
| D4            | GPIO 36 | Y6_GPIO_NUM           |
| D5            | GPIO 39 | Y7_GPIO_NUM           |
| D6            | GPIO 34 | Y8_GPIO_NUM           |
| D7            | GPIO 35 | Y9_GPIO_NUM           |
| XCLK          | GPIO 0  | XCLK_GPIO_NUM         |
| PCLK          | GPIO 22 | PCLK_GPIO_NUM         |
| VSYNC         | GPIO 25 | VSYNC_GPIO_NUM        |
| HREF          | GPIO 23 | HREF_GPIO_NUM         |
| SDA           | GPIO 26 | SIOD_GPIO_NUM         |
| SCL           | GPIO 27 | SIOC_GPIO_NUM         |
| POWER PIN     | GPIO 32 | PWDN_GPIO_NUM         |

---

## Test

-   [Tutorials](https://randomnerdtutorials.com/esp32-cam-video-streaming-web-server-camera-home-assistant/)

---

## Troubleshooting

1. Failed to connect to ESP32: Timed out waiting for packet header
    - <strong>Important: GPIO 0 must be connected to GND so that you’re able to upload code.</strong>
    - Check the output voltage of the ESP32-CAM with 5V
    - Check the output voltage of FTDI Programmer with 5V
2. Camera init failed with error 0x20001 or similar
    - Camera not connected properly
    - Wrong pin assignment in the code: Check the Camera_Model as AI Thinker
    - Not enough power through USB source
    - Faulty FTDI programmer
    - The camera/connector is broken
3. Brownout detector or Guru meditation error
    - Check the less output power
    - Poor quality USB cable
    - USB cable is too long
    - Board with some defect (bad solder joints)
    - Bad computer USB port
    - Or not enough power provided by the computer USB port.

| If you need more information for troubleshooting, please see the troubleshooting guide with the reference site. |

---

## References

-   [Tutorials](https://randomnerdtutorials.com/esp32-cam-take-photo-display-web-server/)

-   [Tutorial Video](https://youtu.be/MicAM_A0_lU)

-   [Troubleshooting](https://randomnerdtutorials.com/esp32-cam-troubleshooting-guide/)

-   [ESPTOOLS](https://github.com/espressif/esptool)

-   Data sheet
    -   [ESP32 series data sheet](https://www.mouser.com/datasheet/2/891/esp-wroom-32_datasheet_en-1223836.pdf)

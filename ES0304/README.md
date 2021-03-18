# WS2812 Adapter Shield for ESP-01 ESP-01S ESP8266

## Table of Contents

-   [Description](#description)
-   [Characteristic](#characteristic)
-   [Connections](#connections)
-   [Test](#test)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Description

This is a tutorial of ESP-01s with the WS2812 Module. The user will be able to control the WS2812 on the web or mobile after finishing this tutorial.
Please check the components for this tutorial.

---

## Characteristic

| Characteristic |                       |
| -------------- | --------------------- |
| Master         | ESP01/01S             |
| Control pin    | GPIO 2                |
| Interface      | 3pins PH2.0 connector |
| support        | 3.7 lithium battery   |

---

## Connections

| Shield        | WS2812  |
| ------------- | ------- |
| Red (VCC)     | 5V      |
| Black (GND)   | GND     |
| Yellow (Data) | Data In |

---

## Test

-   [Tutorial Video](https://youtu.be/tKl5vnxCVcc)
-   [Test code](test/)
-   Required libraries will be updated

**to be updated..**

---

## Troubleshooting

1. Check the installation of ESP8266 Add-on to Arduino IDE

2. Failed to upload the code.

3. For execution this code, Web control interface Files(HTML&JS) should be in the same folder with the below test code. The interface files is in the [test folder](test/) in this page.

4. The positive supply voltage VCC on the board is connected to the VCC on the WS2812 3PIN connector.

5. You could use the external power source if the power of the shield is not enough.

**to be updated..**

---

## References

-   Datasheet

    -   [ESP-01(s)](https://bit.ly/3twNw57)

-   References

    -   [Arduino core for ESP8266 WiFi chip](https://github.com/esp8266/Arduino)
    -   [ESP8266 docs](https://bit.ly/3eVpJYn)

**to be updated..**

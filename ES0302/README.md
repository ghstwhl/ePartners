# DS18B20 shield for ESP8266 ESP-01 ESP-01S

## Table of Contents

-   [Description](#description)
-   [Characteristic](#characteristic)
-   [Test](#test)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Description

This module uses ESP8266-01/ESP-01S as the master control, and DS18B20 as temperature sensor.
ESP8266 collects the temperature in the environment and uploads to the server.
It can be used as temperature collection node for smart home or IOT project.

---

## Characteristic

| Characteristics               |                                                |
| ----------------------------- | ---------------------------------------------- |
| Main control                  | ESP-01/ESP-01s                                 |
| Temperature & Humidity sensor | DS18B20                                        |
| Working voltage               | DC 3.7v-12v (Support for 3.7v lithium battery) |
| Measurement range             | -55°C to + 125°C                               |
| Accuracy of measurement       | ±0.5°C                                         |
| Size                          | 16X20X25mm (L*W*H)                             |

---

## Test

-   [DS18B20 Temperature sensor Using the ESP-01 & DHT](https://youtu.be/oYU0JMWwSuI)
-   Required libraries & test code will be updated

**to be updated..**

---

## Troubleshooting

-   Check your 'COM' port
-   Check your power supply & input voltage
-   Check your board type on IDE

| ![alt text](https://bit.ly/3vGkYI7 'USB to ESP')                                                                                                       |
| ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| If you use a "USB to ESP-01 Adapter board" to upload code, you may encounter some errors                                                               |
| When you encounter an error while uploading code, please refer to [this page](https://www.instructables.com/USB-to-ESP-01-Board-Adapter-Modification/) |

**to be updated..**

---

## References

-   [Advanced Tutorial](https://bit.ly/3f71lDB)

-   Datasheet

    -   [ESP-01(s)](https://bit.ly/3twNw57)

-   References

    -   [Arduino core for ESP8266 WiFi chip](https://github.com/esp8266/Arduino)
    -   [ESP8266 docs](https://bit.ly/3eVpJYn)

-   [Good Article](https://bit.ly/3bVWbIl)

**to be updated..**

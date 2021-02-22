# ESP8266 - CH340 USB to ESP-01 / ESP-01S Wifi Module Adapter

## Table of Contents

-   [Description](#description)
-   [Tips](#tips)
-   [Features](#features)
-   [Schematic](#schematic)
-   [Tutorials](#tutorials)
    -   [Test-environment](#test-environment)
        -   [Hardware](#hardware)
        -   [Software](#software) **..Coming soon..**
    -   [Test](#test) **..Coming soon..**
        -   [Test Code](#test-code) **..Coming soon..**
        -   [Test Result](#test-result) **..Coming soon..**
-   [Troubleshooting](#troubleshooting) **..Coming soon..**
-   [References](#references)

---

## Description

This WiFi relay based on AI-Thinker ESP-01/ 01S WiFi module, we use the GPIO0 of ESP-01/ 01S to control the relay by low level. It’s easy to DIY your smart switch to any device by your phone anywhere with this smart relay.

---

## Tips

-   Mobile phone equipped with WiFi module;
-   Mobile phone and WiFI module equipped with the same router, through the mobile phone APP to control the relay; this mode, the transmission distance depends on the signal router.
-   ESP8266 module has a timeout mechanism, when the phone for some time (the default 180S) did not give instructions to the module, the module will kick off the phone, the computer can send AT + CIPSTO = time to modify this time (Time range 0-7200), such as: AT + CIPSTO = 3600.
-   When the module on the WIFI module is unplugged, USB to TTL module RX, TX, GND pins were connected to the module RX, TX, GND pin, IN +, IN- 5V power supply, then the module can be used as a USB Relays to use, scalability.

---

## Features (Specification)

| Features                        |                                                                                                     |
| ------------------------------- | --------------------------------------------------------------------------------------------------- |
| Working voltage                 | DC 5V-12V                                                                                           |
| Working current                 | &#x2265; 250mA                                                                                      |
| Communication                   | ESP01 or ESP01S Wifi Module                                                                         |
| Serial communication parameters | 9600,8,1,0,                                                                                         |
| Transmission distance           | the maximum transmission distance is 400m(open environment, mobile phone equipped with WiFi module) |
| Load                            | 10A/ 250VAC, 10A/ 30VDC, 10A/ 30VDC, 10A/ 28VDC                                                     |
| Size                            | 37 \* 25mm                                                                                          |

---

## Schematic

![alt text](https://bit.ly/3qLI11A 'ESP8266 Relay')

---

## Tutorials

### Hardware

| ![alt text](https://bit.ly/37z7aVF 'ESP8266-01s') | ![alt text](https://bit.ly/3kbv66F 'ESP8266 Relay') | ![alt text](https://bit.ly/2MgbaD5 'FTDI Converter') |
| ------------------------------------------------- | --------------------------------------------------- | ---------------------------------------------------- |
| ESP8266-01S WiFi Module                           | Relay Shield for ESP-01/ESP-01S                     | USB to TTL Converter                                 |

---

## References

**[Instructions](https://www.instructables.com/ESP0101S-RELAY-MODULE-TUTORIAL/)**

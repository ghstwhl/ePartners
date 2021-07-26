# ESP8266-01s Tutorial (Wifi Connection)

## Table of Contents

-   [Description](#description)
-   [Features](#features)
-   [Pin Decription](#pin-description)
-   [Test](#test)
    -   <b>Built an ESP8266 Web Server</b>
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Description

ESP-01 WiFi module is developed by
encapsulates Tensilica L106 integrates industry
Clock speed support 80 MHz, 160 MHz, supports the RTOS, integrated Wi
The module supports standard IEEE802.11
add modules to an existing device networking, or building a separate network controller.
ESP8266 is high integration wireless SOCs, designed for space and power constrained mobile platform
It provides unsurpassed ability to embed Wi
application, with the lowest cost, and minimal space requirement.

---

## Feature

| Features                                                                                   |
| ------------------------------------------------------------------------------------------ |
| 802.11 b/g/n                                                                               |
| Integrated low power 32-bit MCU                                                            |
| Integrated 10-bit ADC                                                                      |
| Integrated TCP/IP protocol stack                                                           |
| Integrated TR switch, balun, LNA, power amplifier and matching network                     |
| Integrated PLL, regulators, and power management units                                     |
| Supports antenna diversity                                                                 |
| Wi-Fi 2.4 GHz, support WPA/WPA2                                                            |
| Support STA/AP/STA+AP operation modes                                                      |
| Support Smart Link Function for both Android and iOS devices                               |
| SDIO 2.0, (H) SPI, UART, I2C, I2S, IRDA, PWM, GPIO                                         |
| STBC, 1x1 MIMO, 2x1 MIMO                                                                   |
| A-MPDU & A-MSDU aggregation and 0.4s guard interval                                        |
| Deep sleep power <10uA, Power down leakage current < 5uA                                   |
| Wake up and transmit packets in < 2ms                                                      |
| Standby power consumption of < 1.0mW (DTIM3)                                               |
| +20dBm output power in 802.11b mode                                                        |
| Operating temperature range -40C ~ 125C                                                    |
| 1MB Flash Memory                                                                           |
| Can be used as Station or Access Point or both combined                                    |
| Supports serial communication hence compatible with many development platform like Arduino |
| Can be programmed using Arduino IDE or AT-commands or Lua Script                           |

---

## Pin Description

|![alt text](https://bit.ly/36YC1dB 'ESP-01 pinout')

| NO. | Pin Name | Alternate Name | Normally used for                                      |
| --- | -------- | -------------- | ------------------------------------------------------ |
| 1   | GND      | -              | Connected to the ground of the circuit                 |
| 2   | TX       | GPIO-1         | Connected to RX pin of programmer/uC to upload program |
| 3   | GPIO-2   | -              | General purpose Input/Output pin                       |
| 4   | CH_EN    | -              | Chip Enable - Active high                              |
| 5   | GPIO-0   | Flash          | General purpose Input/Output pin                       |
| 6   | Reset    | -              | Resets the module                                      |
| 7   | RX       | GPIO-3         | General purpose Input/Output pin                       |
| 8   | VCC      | -              | Connect to +3.3V only                                  |

---

## Test

It's an easy tutorial to start ESP8266

-   [Built an ESP8266 Web Server Tutorial](https://randomnerdtutorials.com/esp8266-web-server/)
-   [Test code](test/esp-01s.ino)

## Troubleshooting

1. If you cannot upload the code, check your COM port in the <b>Device manager</b>.
2. EN pin (or CHPD pin) must be connected to 3.3V
3. Before the code is upload to ESP-01s, GPIO 0 pin must be connected to GND.
4. After uploading the code, GPIO 0 pin must be disconnected from GND. -->

## References

-   Datasheet
    -   [ESP-01(s)](https://bit.ly/3twNw57)
-   Tutorial
    -   [ESP-01S AT Commands Firmware Flashing](https://bit.ly/30U7Ukw)
-   References
    -   [Arduino core for ESP8266 WiFi chip](https://github.com/esp8266/Arduino)
    -   [ESP8266 docs](https://arduino-esp8266.readthedocs.io/en/latest/esp8266wifi/readme.html)

to be updated...

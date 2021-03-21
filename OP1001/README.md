# WeMos D1 mini - NodeMcu development board based ESP8266

## Table of Contents

-   [Descriptions](#descriptions)
-   [features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

Wemos D1 mini is like a "little Arduino with wifi" for a great price. It's based around the ESP8266, has one analogue port and 11 digital ports. It's programmed via micro-USB (or remote flash via wifi). You can use it with the Arduino IDE, micropython or NodeMCU.

It runs from 5V or 3.3V. Logic levels are 3.3V for all ports.

If you use the Arduino IDE, there are a lot of example sketches already provided. This makes life relatively easy to be able to do what you want.

---

## Features (Specifications)

| Features                                               |
| ------------------------------------------------------ |
| Embeded ESP8266-12F with PCB antena                    |
| Flash: 4M                                              |
| Wi-Fi in standard 802.11 b/g/                          |
| WiFi modes: AP (Access Point), STA (Standalone), AP+ST |
| Supports TKIP, WEP, CRC, CCMP, WPA/WPA2, WP            |
| Supply voltage: 3.3V (or 5V via USB                    |
| CPU: RISC 80MHz (supports up to 160MHz)                |
| 9 GPIO - PWM / I2C / SPI / 1-Wir                       |
| Max current on I/O pins: 12m                           |
| Recommended current on I/O pins: 6m                    |
| USB-UART converter - CH340                             |
| ADC - 10-bi                                            |
| 16 pins in 2,54mm raster - breadboard compatibl        |
| micro USB                                              |
| Size: 34 x 25m                                         |
| LED connected to GPIO2 (D4                             |

---

## Pins

| Pin | Function                     | ESP-8266 Pin |
| --- | ---------------------------- | ------------ |
| TX  | TXD                          | TXD          |
| RX  | RXD                          | RXD          |
| A0  | Analog input, max 3.2V       | A0           |
| D0  | IO                           | GPIO16       |
| D1  | IO, SCL                      | GPIO5        |
| D2  | IO, SDA                      | GPIO4        |
| D3  | IO, 10k Pull-up              | GPIO0        |
| D4  | IO, 10k Pull-up, BUILTIN_LED | GPIO2        |
| D5  | IO, SCK                      | GPIO14       |
| D6  | IO, MISO                     | GPIO12       |
| D7  | IO, MOSI                     | GPIO13       |
| D8  | IO, 10k Pull-down, SS        | GPIO15       |
| G   | Ground                       | GND          |
| 5V  | 5V                           | -            |
| 3V3 | 3.3V                         | 3.3V         |
| RST | Reset                        | RST          |

---

## Test

-   [Tutorials I](https://www.instructables.com/Wemos-ESP8266-Getting-Started-Guide-Wemos-101/)
-   For more tutorials, please refer to the references section in this page.

**to be updated..**

---

## Troubleshooting

-   If you use this board with breadboard, the soldering should be properly.

**to be updated..**

---

## References

-   [WEMOS Docs](https://www.wemos.cc/en/latest/index.html)

-   [Tutorial Video I](http://bit.ly/Wemos-D1-mini-first-look)

-   [Tutorial Video II](https://www.youtube.com/watch?v=G73fiaOpUAc)

-   [Tutorial Video III](https://www.youtube.com/watch?v=TKN9WmunCQU)

**to be updated..**

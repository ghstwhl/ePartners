# TCS230 TCS3200 Color Recognition Sensor Detector

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The TCS230 color detector measures three primary colors Red, Green and Blue and also has a separate white light detector. Since any color can be created from different levels of these primary colors, you can find out the color composition of a light source.
The four LEDs on the breakout board (shown below) are there to illuminate the subject with an even light source, making measurement more reliable.

---

### Difference between TC230 and TCS3200

| Parameter             | TCS230     | TCS3200/[TCS3210] | Units |
| --------------------- | ---------- | ----------------- | ----- |
| Number of photodiodes | 64         | 64 / [24]         | -     |
| Power on current      | 2 (max 3)  | 1.4 (max 2)       | mA    |
| Power down current    | 7 (max 15) | 0.1 (max 0.1)     | uA    |
| min operating temp.   | 0          | -40               | °C    |

---

## Features (Specifications)

| Features (Specifications)   |                                  |
| --------------------------- | -------------------------------- |
| Voltage Supply (VDD)        | 2V7 ~ 5V5                        |
| Abs.Max VDD                 | -0.3V ~ 6V3                      |
| Measurement range           | Approx. 300nm to 980nm [3]       |
| Output interface type       | Frequency pin o/p single pin [2] |
| Logic Levels                | CMOS or TTL                      |
| Logic input voltage (L,H)   | 0V0 ~ 0V8, 2V0 ~ VDD             |
| Logic output voltage (L,H)  | 0V4, 4.5 (for VDD=5V)            |
| Output frequency Scale 100% | 600kHz (typ) [1][2]              |
| Output frequency Scale 20%  | 120kHz (typ) [1][2]              |
| Output frequency Scale 2%   | 12kHz (typ) [1][2]               |
| Active current              | 2mA (typ), 3mA (max)             |
| Power down current          | 7uA (typ), 15uA (max)            |
| Operating temperature       | -40°C ~ 70°C                     |

---

## Pins

![alt text](https://bit.ly/3w0GkjW 'TCS230')

| Pin Name | Description                |
| -------- | -------------------------- |
| GND      | Ground                     |
| OE       | Output Enable              |
| SO       | Frequency scaling          |
| S1       | Frequency scaling          |
| S2       | Select the color array     |
| S3       | Select the color array     |
| OUT      | TTL level square wave      |
| VCC      | Power supply. 2.7V to 5.5V |

## Test

-   [Tutorial I](https://www.best-microcontroller-projects.com/tcs230.html#L1573)
-   [Tutorial II](http://bit.ly/Color-Sensing-Tutorial)
-   [Tutorial III](http://bit.ly/Color-Sensing-Tutorial-3)

-   [Tutorial Video I](https://youtu.be/CPUXxuyd9xw)
-   [Tutorial Video II](https://youtu.be/hDAOGcI9cv4)
-   [Tutorial Video III](https://youtu.be/4Zu4rwwPoCg)

    **to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [TCS230 TCS3200 Datasheet](https://bit.ly/3lTHKaY)

**to be updated..**

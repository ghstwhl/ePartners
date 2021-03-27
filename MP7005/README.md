# Ultrasonic Module HC SR04 Distance Measuring Sensor

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The HC-SR04 ultrasonic sensor uses sonar to determine distance to an object like bats do. It offers excellent non-contact range detection with high accuracy and stable readings in an easy-to-use package. It comes complete with ultrasonic transmitter and receiver modules.

---

## Features (Specifications)

| Features (Specifications)      |
| ------------------------------ | ------------------------------------------------------ |
| Operating voltage              | +5V                                                    |
| Output signal                  | Electric frequency signal, high-level 5V, low-level 0V |
| Static current                 | Less than 2mA                                          |
| Theoretical Measuring Distance | 2cm to 450cm                                           |
| Practical Measuring Distance   | 2cm to 80cm                                            |
| Accuracy                       | 3mm                                                    |
| Measuring angle covered        | <15°                                                   |
| Operating Current              | <15mA                                                  |
| Operating Frequency            | 40Hz                                                   |
| Input trigger signal           | 10uS TTL impulse                                       |
| Echo signal                    | output TTL PWL signal                                  |

---

## Pins

![alt text](https://bit.ly/3w3vj1b)

| Pin Number | Pin Name | Description                                                        |
| ---------- | -------- | ------------------------------------------------------------------ |
| 1          | Vcc      | The Vcc pin powers the sensor, typically with +5V                  |
| 2          | Trigger  | Trigger pin is an Input pin. This pin has to be kept high for 10us |
|            |          | to initialize measurement by sending US wave.                      |
| 3          | Echo     | Echo pin is an Output pin.                                         |
|            |          | This pin goes high for a period of time                            |
|            |          | which will be equal to the time taken for the US wave              |
|            |          | to return back to the sensor.                                      |
| 4          | Ground   | This pin is connected to the Ground of the system.                 |

---

## Test

-   [Tutorial I](https://bit.ly/3lTJ7qi)
-   [Tutorial II](https://randomnerdtutorials.com/complete-guide-for-ultrasonic-sensor-hc-sr04/)
-   [Tutorial III](https://howtomechatronics.com/tutorials/arduino/ultrasonic-sensor-hc-sr04/)

-   [Tutorial Video I](https://youtu.be/ZejQOX69K5M)
-   [Tutorial Video II](https://youtu.be/6F1B_N6LuKw)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [Datasheet](https://bit.ly/3svTa7t)

**to be updated..**

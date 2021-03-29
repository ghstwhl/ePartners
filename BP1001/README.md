# L298N Dual Bridge DC Stepper Motor Driver Board

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The L298N driver module, using ST's L298N chip can directly drive two 3-30V DC motor, and provides a 5V output interface can 5V single-chip circuitry to supply, support 3.3VMCU control, you can easily control the DC motor speed and direction, you can also control the 2-phase stepper motor, smart car essential.

---

## Features (Specifications)

| Features (Specifications)                        |                                                                                     |
| ------------------------------------------------ | ----------------------------------------------------------------------------------- |
| Driver                                           | L298N Dual H Bridge DC Motor Driver IC                                              |
| Driven part of the terminal supply area Vs       | +5 V ~ +35 V (such as the need to take power within the board the supply area Vs:   |
|                                                  | +7 V ~ +35V)                                                                        |
| Driven part of the peak current Io               | 2A                                                                                  |
| The logical part of the terminal supply area Vss | +5 V ~ +7 V (can take power within the board +5 V)                                  |
| The logical part of the operating current range  | 0 ~ 36mA                                                                            |
| Control signal input voltage range               | Low:-0.3V                                                                           |
|                                                  | High: 2.3V                                                                          |
| Enable signal input voltage range                | Low: -0.3                                                                           |
|                                                  | High: 2.3V                                                                          |
| Maximum power consumption                        | 20W (when the temperature T = 75 Deg C)                                             |
| Storage temperature                              | -25 Deg C ~ +130 Deg C                                                              |
| Other Extensions                                 | Control of direction indicators the logic part of the plate to take power interface |
| Driver Board Size                                | 55mm _ 60mm _ 30mm                                                                  |
| Drive plate Weight                               | 33g                                                                                 |

---

## Pins

![alt text](https://bit.ly/3rB6dDn 'L298N')

| Pin   | Description                                                                                                   |
| ----- | ------------------------------------------------------------------------------------------------------------- |
| Out 1 | Motor A lead out                                                                                              |
| Out 2 | Motor A lead out                                                                                              |
| Out 3 | Motor B lead out                                                                                              |
| Out 4 | Mo (Can actually be from 5v-35v, just marked as 12v)                                                          |
| GND   | Ground                                                                                                        |
| 5v    | 5v input unnecessary if your power source is 7v-35v if the power source is 7v-35v then it can act as a 5v out |
| EnA   | Enables PWM signal for Motor A                                                                                |
| In1   | Enable Motor A                                                                                                |
| In2   | Enable Motor A                                                                                                |
| In3   | Enable Motor B                                                                                                |
| In4   | Enable Motor B                                                                                                |
| EnB   | Enables PWM signal for Motor B                                                                                |

---

## Test

-   [Tutorial I](https://bit.ly/39sEFKh)
-   [Tutorial II](https://www.instructables.com/Control-DC-and-stepper-motors-with-L298N-Dual-Moto/)
-   [Tutorial III](https://dronebotworkshop.com/dc-motors-l298n-h-bridge/)

-   [Tutorial Video I](https://youtu.be/I7IFsQ4tQU8)
-   [Tutorial Video II](https://youtu.be/dyjo_ggEtVU)
-   [Tutorial Video III](https://youtu.be/Ey4xoG970Go)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [L298N Manual](https://bit.ly/3flXjHr)
-   [L298 Datasheet](https://bit.ly/3u1pxLJ)

**to be updated..**

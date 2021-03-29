# 28BYJ-48 Stepper Motor

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

Stepper motors are great motors for position control. They are a special type of brushless motors that divides a full rotation into a number of equal “steps”. They are usually found in desktop printers, 3D printers, CNC milling machines, and anything else that requires precise positioning control.

The motor usually comes with a ULN2003 based driver board.

The ULN2003 is one of the most common motor driver ICs, consisting of an array of 7 Darlington transistor pairs, each pair is capable of driving loads of up to 500mA and 50V. Four out of seven pairs are used on this board.

---

## Features (Specifications)

| Features (Specifications)   |                                       |
| --------------------------- | ------------------------------------- |
| Model                       | 28BYJ-48 – 5V                         |
| Motor type                  | Permanent Magnet Gear Motor           |
| Rated voltage               | 5VDC                                  |
| Number of Phase             | 4                                     |
| Coil Resistance             | 50 Ohms                               |
| Coil Type                   | Unipolar                              |
| Diameter – shaft            | 0.197″ (5.00 mm)                      |
| Length – shaft and bearing  | 0.394″ (10 mm)                        |
| Speed Variation Ratio       | 1/64                                  |
| Stride Angle                | 5.625° /64                            |
| Step angle                  | Half step mode (recommended): 0.0879° |
|                             | Full step mode: 0.176°                |
| Steps per revolution        | Half step mode: 4096 (see note)       |
|                             | Full step mode: 2048                  |
| Frequency                   | 100Hz                                 |
| DC resistance               | 50Ω±7%(25℃)                           |
| Idle In-traction Frequency  | > 600Hz                               |
| Idle Out-traction Frequency | > 1000Hz                              |
| In-traction Torque          | >34.3mN.m(120Hz)                      |
| Self-positioning Torque     | >34.3mN.m                             |
| Friction torque             | 600-1200 gf.cm                        |
| Pull in torque              | 300 gf.cm                             |
| Insulated resistance        | >10MΩ(500V)                           |
| Insulated electricity power | 600VAC/1mA/1s                         |
| Insulation grade            | A                                     |
| Rise in Temperature         | <40K(120Hz)                           |
| Noise                       | <35dB(120Hz,No load,10cm)             |

---

## Pins

| ![alt text](https://bit.ly/3dfYyVP '28BYJ-48') | ![alt text](https://bit.ly/3rzcvU2 '28BYJ-48') |
| ---------------------------------------------- | ---------------------------------------------- |

| No. | Pin Name | Wire Color | Description                                                                                                                                                                                             |
| --- | -------- | ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | Coil 1   | Orange     | : This Motor has a total of four coils. One end of all the coils are connect to +5V (red) wire and the other end of each coil is pulled out as wire colors Orange, Pink, Yellow and Blue respectively : |
| 2   | Coil 2   | Pink       | ^^                                                                                                                                                                                                      |
| 3   | Coil 3   | Yellow     | ^^                                                                                                                                                                                                      |
| 4   | Coil 4   | Blue       | ^^                                                                                                                                                                                                      |
| 5   | +5V      | Red        | We should supply +5V to this wire, this voltage will appear across the coil that is grounded                                                                                                            |

---

## Test

-   [Tutorial I](https://bit.ly/3sAhcyh)
-   [Tutorial II](https://bit.ly/3m4XPux)
-   [Tutorial III](https://bit.ly/3wd5bAO)

-   [Tutorial Video I](https://youtu.be/avrdDZD7qEQ)
-   [Tutorial Video II](https://youtu.be/4iRvjBwAzrM)
-   [Tutorial Video III](https://youtu.be/lmMTsbSbHC8)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [ULN2003 Datasheet](https://bit.ly/3dlhOBc)
-   [Article 1](https://bit.ly/2QRyqZZ)
-   [Article 2](https://bit.ly/2PCV0oG)

**to be updated..**

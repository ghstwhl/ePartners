# Load Cell HX711 Weighing Sensors

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

A load cell is an application of strain measurements relating to weight measurement. A load is applied to a strain gauge, which causes the gauge to strain a certain amount and output a voltage proportional to the applied load. This relationship between strain and voltage is used in many applications where weight measurement is important. Load cells are very common because of their linearity, cost effectiveness, and their ease of implementation. In this tutorial, I will introduce an Arduino-compatible load cell that exemplifies all of the aforementioned advantages. I will also introduce calibration with known masses to create a powerful and accurate weighing system that can be used for highly accurate measurement purpose such as: chemistry, horticulture, cooking, and much more!

---

## Features (Specifications)

| Features (Specifications)                                                               |
| --------------------------------------------------------------------------------------- |
| Two selectable differential input channels                                              |
| On-chip active low noise PGA with selectable gain of 32, 64 and 128                     |
| On-chip power supply regulator for load-cell andADC analog power supply                 |
| On-chip oscillator requiring no externalcomponent with optional external crystal        |
| On-chip power-on-reset                                                                  |
| Simple digital control and serial interface: pin-driven controls, no programming needed |
| Selectable 10SPS or 80SPS output data rate                                              |
| Simultaneous 50 and 60Hz supply rejection                                               |
| Current consumption:normal operation < 1.5mA, power down < 1uA                          |
| Operation supply voltage range: 2.6V to 5.5V                                            |
| Operation temperature range: -40℃ to +85℃                                               |

---

## Pins

![alt text](https://bit.ly/2PctjTC 'Pinout')

| HX711 | Arduino Uno |
| ----- | ----------- |
| VCC   | 5V          |
| GND   | GND         |
| SCK   | D5          |
| DT    | D6          |

| Load Cell | HX711 |
| --------- | ----- |
| E+        | RED   |
| E-        | BLACK |
| A-        | WHITE |
| A+        | GREEN |

---

## Test

-   [Tutorial I](https://bit.ly/32I7gaF)
-   [Tutorial II](https://bit.ly/Weighing-Sensor-Tutorial)
-   [Tutorial III](https://bit.ly/2QS1Wyx)

-   [Tutorial Video I](https://youtu.be/pZpzdu97JYw)
-   [Tutorial Video II](https://youtu.be/S12Mp8gDJmI)
-   [Tutorial Video III](https://youtu.be/ZwJw_BtFiUc)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [HX711 Datasheet](https://bit.ly/3tNce1y)

**to be updated..**

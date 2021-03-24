# TCRT5000 Infrared Reflective Sensor / Line Track Module

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

This IR reflective sensor utilizes a TCRT5000 to detect color and distance. It emits IR and then detects if it receives the echo. This sensor is often used in line following robots, auto data logging on utility meters, because this module can sense if a surface is white or black.
The measuring distance range from 1mm to 8mm, and the central point is about 2.5mm. There is also an on-board potentiometer to adjust the sensitivity. The infrared diode will emitting the infrared continuously when the module connect to the power, when the emitted infrared light has not been reflected or the strength is not big enough,the module will in the off state, at this time, D0 output logic HIGH and the signal indicate LED off.

---

## Features (Specifications)

| Features(Specifications)                         |
| ------------------------------------------------ |
| Supply Voltage: 3.3V~5V                          |
| Detect distance: 1mm-8mm                         |
| Focus Range: 2.5 mm                              |
| Driving Ability: > 15 mA                         |
| Digital Outputs LOW when objects detected        |
| Output: digital switch outputs (0 and 1)         |
| On-board indicator LED to show the results       |
| On-board potentiometer to adjust the sensitivity |
| On-board LM393 chip                              |

---

## Pins

![alt text](https://bit.ly/3skGuQE 'TCRT5000')

| TCRT5000 Module | Arduino Uno |
| --------------- | ----------- |
| VCC             | 5V          |
| GND             | GND         |
| DO              | Digital pin |
| AO              | Analog pin  |

---

## Test

-   [Tutorial I](https://www.instructables.com/How-to-Use-TCRT5000-IR-Sensor-Module-With-Arduino-/)
-   [Tutorial II](https://bit.ly/3lLsixV)

-   [Tutorial Video I](https://www.youtube.com/watch?v=LuX_ZGIRCzo)
-   [Tutorial Video II](https://www.youtube.com/watch?v=eDKbRlADvA0)
-   [Tutorial Video III](https://youtu.be/ohBGHPFQeuk)

    **to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [TCRT500 Data sheet](https://bit.ly/397eetu)
-   [LM393 Datasheet](https://bit.ly/2PngwO8)

**to be updated..**

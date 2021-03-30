# A4988 Stepper Motor Driver Module

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The A4988 is a microstepping driver for controlling bipolar stepper motors which has built-in translator for easy operation. This means that we can control the stepper motor with just 2 pins from our controller, or one for controlling the rotation direction and the other for controlling the steps.

The Driver provides five different step resolutions: full-step, haft-step, quarter-step, eight-step and sixteenth-step. Also, it has a potentiometer for adjusting the current output, over-temperature thermal shutdown and crossover-current protection.

---

## Features (Specifications)

| Features (Specifications)                                               |
| ----------------------------------------------------------------------- |
| Low RDS (On) Output                                                     |
| Automatic current decay mode detection / selection                      |
| Mix with slow current decay modes                                       |
| Synchronous rectification for low power dissipation                     |
| Internal UVLO                                                           |
| Cross-current protection                                                |
| 3.3 and 5 V compatible logic supply                                     |
| Thermal shutdown circuitry                                              |
| Ground fault protection                                                 |
| Load short-circuit protection                                           |
| Optional step five modes: full, 1/2step, 1/4step, 1/8step and 1/16 step |

---

## Pins

| ![alt text](https://bit.ly/3dhSooh 'A4988') | ![alt text](https://bit.ly/3wfS7Ll 'A4988') |
| ------------------------------------------- | ------------------------------------------- |

| Pin Name       | Description                           |
| -------------- | ------------------------------------- |
| VDD & GND      | Connected to 5V and GND of Controller |
| VMOT & GND     | Used to power the motor               |
| 1A, 1B, 2A, 2B | Connected to the 4 coils of motor     |
| DIRECTION      | Motor Direction Control pin           |
| STEP           | Steps Control Pin                     |
| MS1, MS2, MS3  | Microstep Selection Pins              |
| SLEEP          | Pins For Controlling Power States     |
| RESET          |                                       |
| ENABLE         |                                       |

---

## Test

-   [Tutorial I](https://bit.ly/3ft87ni)
-   [Tutorial II](http://bit.ly/How-To-Control-Stepper-Motor-with-A4988)
-   [Tutorial III](http://bit.ly/A4988-Stepper-Motor-Driver-Carrier)
-   [Tutorial IV](https://bit.ly/3sCy1bD)

-   [Tutorial Video I](https://youtu.be/KM-5PYfRlso)
-   [Tutorial Video II](https://youtu.be/5CmjB4WF5XA)
-   [Tutorial Video III](https://youtu.be/hl5AzPA1uB8)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [A4988 Datasheet](https://bit.ly/3rKR1DX)

**to be updated..**

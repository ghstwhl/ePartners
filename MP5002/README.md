# Current Sensor 30A (ACS712)

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

Reading Sensing and Controlling current flow is a requirements in a wide variety of application including, over-current protection circuits, switching mode, battery chargers, power supplies, digital watt meter and programmable current source, etc.. The ACS721 current reading module is based on ACS712 Sensor which can detect AC, DC current signal accurately.

The maximum AC / DC can be detected using ACS712 will reach 30 amp and present current signal can read via analog IO port of Arduino, Product available for this module are 30A, 20A, 5A. for this demonstration we will used the ACS712 30A.

---

## Features (Specifications)

| Features                                                                                              |
| ----------------------------------------------------------------------------------------------------- |
| Current sensor chips: ACS712ELC-30A                                                                   |
| Pin 5V power supply, on-board power indicator                                                         |
| The module can measure the positive and negative 30 amps, corresponding to the analog output 66mV / A |
| No test current through the output voltage is VCC / 2                                                 |
| PCB board size: 31 (mm) x13 (mm)                                                                      |

---

## Pins

| ![alt text](https://bit.ly/3clqR5W 'pinout') | ![alt text](https://bit.ly/3clpeFl 'pinout') |
| -------------------------------------------- | -------------------------------------------- |

| Pin Number | Pin Name | Pin Description                           |
| ---------- | -------- | ----------------------------------------- |
| 1 & 2      | IP+      | +ve terminals for sensing current         |
| 3 & 4      | IP-      | -ve terminals for sensing current         |
| 5          | GND      | Signal Ground                             |
| 6          | FILTER   | External Capacitor (to set the bandwidth) |
| 7          | VIOUT    | Analog Output                             |
| 8          | VCC      | Power Supply                              |

**For more features, please refer to the datasheet in [this section](#references)**

---

## Test

-   [Tutorial I](https://create.arduino.cc/projecthub/SurtrTech/measure-any-ac-current-with-acs712-70aa85)
-   [Tutorial II](https://electronoobs.com/eng_arduino_tut118.php)
-   [Tutorial III](https://www.engineersgarage.com/arduino/acs712-current-sensor-with-arduino/)

-   [Tutorial Video I](https://youtu.be/VjV_8EctLBM)
-   [Tutorial Video II](https://youtu.be/GcSFvG1DFB0)
-   [Tutorial Video III](https://youtu.be/3C33DpcSwIw)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [For more information](https://bit.ly/2QA7DRD)
-   [ACS712 Datasheet](https://bit.ly/3ff57KZ)

**to be updated..**

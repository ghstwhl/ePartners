# IR Infrared Slotted Optical Speed Measuring Sensor Module

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

This module integrates DHT22 (or AM2302) sensor and other required components on a small PCB. The DHT22 sensor includes a resistive-type humidity measurement component, an NTC temperature measurement component and a high-performance 8-bit microcontroller inside, and provides calibrated digital signal output. It has high reliability and excellent long-term stability, thanks to the exclusive digital signal acquisition technique and temperature & humidity sensing technology.

DHT22 is a upgraded version of DHT11, and provides better resolution and accuracy. The only drawback, comparing to DHT11, is that its maximum sampling rate is even lower: with DHT11 you could request data for every one second, but with DHT22, you could request data for every two seconds.

### Difference between DHT22 Sensor and Module

The DHT22 sensor is the successor of the DHT11 module, it can either be purchased as a sensor or as a module. Either way the performance of the sensor is same. The sensor will come as a 4-pin package out of which only three pin will be used whereas the module will come with just three pins as shown in the DHT22 pinout above.

The only difference between the sensor and module is that the module will have a filtering capacitor and pull-up resistor inbuilt, and for the sensor you have to use them externally if required.

**_The module is slightly costly than the DHT11, but it has a higher measuring range and slightly better accuracy._**

---

## Features (Specifications)

| Features          |                                          |
| ----------------- | ---------------------------------------- |
| Operating Voltage | 3.5V to 5.5V                             |
| Operating current | 0.3mA (measuring) 60uA (standby)         |
| Output            | Serial data                              |
| Temperature Range | -40°C to 80°C                            |
| Humidity Range    | 0% to 100%                               |
| Resolution        | Temperature and Humidity both are 16-bit |
| Accuracy          | ±0.5°C and ±1%                           |

---

## Pins

| DHT22 Module | Arduino                                                   |
| ------------ | --------------------------------------------------------- |
| Vcc(+)       | Power supply 3.5V to 5.5V                                 |
| Data         | Outputs both Temperature and Humidity through serial Data |
| Ground(-)    | Connected to the ground of the circuit                    |

---

## Test

-   [Tutorial I](http://cactus.io/hookups/sensors/temperature-humidity/dht22/hookup-arduino-to-keyes-dht22-temp-humidity-module)
-   [Tutorial 2](https://www.makerguides.com/dht11-dht22-arduino-tutorial/)

-   [Tutorial Video I](https://youtu.be/oi_GPSLjgBY)
-   [Tutorial Video II](https://youtu.be/BCB1zzRWGF8)
-   [Tutorial Video III](https://youtu.be/1A4-6hDARQc)
-   [Tutorial Video IV](https://youtu.be/IPrEjQn_cTM)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [Good Article](http://bit.ly/Temperature-Sensors-comparison)
-   [Data sheet](https://bit.ly/3f7q1vB)

**to be updated..**

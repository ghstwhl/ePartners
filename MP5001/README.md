# DHT11 Digital Temperature And Humidity Sensor Module

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The DHT11 is a commonly used Temperature and humidity sensor. The sensor comes with a dedicated NTC to measure temperature and an 8-bit microcontroller to output the values of temperature and humidity as serial data. The sensor is also factory calibrated and hence easy to interface with other microcontrollers.

The sensor can measure temperature from 0°C to 50°C and humidity from 20% to 90% with an accuracy of ±1°C and ±1%. So if you are looking to measure in this range then this sensor might be the right choice for you.

### Difference between DHT 11 Sensor and module

The DHT11 sensor can either be purchased as a sensor or as a module. Either way, the performance of the sensor is same. The sensor will come as a 4-pin package out of which only three pins will be used whereas the module will come with three pins as shown above.

The only difference between the sensor and module is that the module will have a filtering capacitor and pull-up resistor inbuilt, and for the sensor, you have to use them externally if required.

---

## Features (Specifications)

| Features          |                                          |
| ----------------- | ---------------------------------------- |
| Operating Voltage | 3.5V to 5.5V                             |
| Operating current | 0.3mA (measuring) 60uA (standby)         |
| Output            | Serial data                              |
| Temperature Range | 0°C to 50°C                              |
| Humidity Range    | 20% to 90%                               |
| Resolution        | Temperature and Humidity both are 16-bit |
| Accuracy          | ±1°C and ±1%                             |

---

## Pins

![alt text](https://bit.ly/2P7fPsk 'pinout')

| DHT22 Module | Arduino                                                   |
| ------------ | --------------------------------------------------------- |
| Vcc(+)       | Power supply 3.5V to 5.5V                                 |
| Out(Data)    | Outputs both Temperature and Humidity through serial Data |
| Ground(-)    | Connected to the ground of the circuit                    |

---

## Test

-   [Tutorial I](https://www.instructables.com/DHT11-Humidity-Sensor-Module-Interface-With-Arduin/)
-   [Tutorial II](https://create.arduino.cc/projecthub/techno_z/dht11-temperature-humidity-sensor-98b03b)
-   [Tutorial III](http://www.uugear.com/portfolio/dht11-humidity-temperature-sensor-module/)

-   [Tutorial Video I](https://youtu.be/OogldLc9uYc)
-   [Tutorial Video II](https://youtu.be/ObjikQDh1Zc)
-   [Tutorial Video III](https://youtu.be/oZ-oFY6TiPw)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [Good Article](http://bit.ly/Temperature-Sensors-comparison)
-   [Data sheet](https://bit.ly/3fhdVQG)
-   [DHT11 Product manual](https://bit.ly/31jZ6V7)

**to be updated..**

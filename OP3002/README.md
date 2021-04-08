# GY-521 MPU6050 3-Axis Analog Gyro Sensors + Accelerometer breakout board

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The MPU6050 is a Micro Electro-Mechanical Systems (MEMS) which consists of a 3-axis Accelerometer and 3-axis Gyroscope inside it. This helps us to measure acceleration, velocity, orientation, displacement and many other motion related parameter of a system or object. This module also has a (DMP) Digital Motion Processor inside it which is powerful enough to perform complex calculation and thus free up the work for Microcontroller.

The module also have two auxiliary pins which can be used to interface external IIC modules like an magnetometer, however it is optional. Since the IIC address of the module is configurable more than one MPU6050 sensor can be interfaced to a Microcontroller using the AD0 pin. This module also has well documented and revised libraries available hence it’s very easy to use with famous platforms like Arduino. So if you are looking for a sensor to control motion for your RC Car, Drone, Self balancing Robot, Humanoid, Biped or something like that then this sensor might be the right choice for you.

---

## Features (Specifications)

| Features (Specifications)                                         |                           |
| ----------------------------------------------------------------- | ------------------------- |
| MEMS 3-aixs accelerometer                                         |                           |
| 3-axis gyroscope values combined                                  |                           |
| Power Supply                                                      | 3-5V                      |
| Communication                                                     | I2C protocol              |
| Built-in 16-bit ADC provides high accuracy                        |                           |
| Built-in DMP provides high computational power                    |                           |
| Can be used to interface with other IIC devices like magnetometer |                           |
| Configurable IIC Address                                          |                           |
| In-built Temperature sensor                                       |                           |
| Chip built-in 16bit AD converter, 16-bit data output              |                           |
| Gyroscope range                                                   | ± 250 500 1000 2000 ° / s |
| Acceleration range                                                | ± 2 ± 4 ± 8 ± 16g         |
| Immersion Gold PCB machine welding process to ensure quality      |                           |
| Pin pitch 2.54mm                                                  |                           |

---

## Pins

| ![alt text](https://bit.ly/3dPodoS 'GY-521') | ![alt text](https://bit.ly/39UP2Xg 'GY-521') |
| -------------------------------------------- | -------------------------------------------- |

| Pin Name                     | Description                                                                                  |
| ---------------------------- | -------------------------------------------------------------------------------------------- |
| Vcc                          | Provides power for the module, can be +3V to +5V                                             |
|                              | Typically +5V is used                                                                        |
| Ground                       | Connected to Ground of system                                                                |
| Serial Clock (SCL)           | Used for providing clock pulse for I2C Communication                                         |
| Serial Data (SDA)            | Used for transferring Data through I2C communication                                         |
| Auxiliary Serial Data (XDA)  | Can be used to interface other I2C modules with MPU6050 It is optional                       |
| Auxiliary Serial Clock (XCL) | Can be used to interface other I2C modules with MPU6050. It is optional                      |
| AD0                          | If more than one MPU6050 is used a single MCU, then this pin can be used to vary the address |
| Interrupt (INT)              | Interrupt pin to indicate that data is available for MCU to read                             |

## Test

-   [Tutorial I](https://bit.ly/3fQJMbd)
-   [Tutorial II](https://bit.ly/3dLcHKW)
-   [Tutorial III](https://bit.ly/3wCykG8)

-   [Tutorial Video I](https://youtu.be/wTfSfhjhAU0)
-   [Tutorial Video II](https://youtu.be/y5X2zwbO6e4)
-   [Tutorial Video III](https://youtu.be/UxABxSADZ6U)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [MPU6050 Datasheet](https://bit.ly/3uxXqUM)

**to be updated..**

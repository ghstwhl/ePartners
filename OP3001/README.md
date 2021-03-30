# SG90 360 Degree Continuous Rotation Servo

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pin](#pin)
-   [Troubleshooting](#troubleshooting)
-   [Reference](#reference)

---

## Descriptions (Important Information)

This factory modified version of the extremely common SG90 servo is a very basic continuous rotation servo. The servo offers an inexpensive and easy to control method of getting your small turret spinning or miniature robot moving. This servo can work with both 5 V and 3.3 V servo signals and has a standard servo connector.

The servo can be controlled using a direct connection to a single microcontroller I/O line without any additional electronics, which makes it a great miniature actuator for beginner robotics projects. Just drive it like a normal servo.

**Note:**

-   This servo has <strong>no positional awareness</strong> so that shaft can rotate freely.
-   You don't need to modify it yourself. It is factory modified.

## Features (Specifications)

| Features (Specifications) |                                          |
| ------------------------- | ---------------------------------------- |
| Dimensions                | 22.6 x 12.2 x 30 mm /0.89x0.48x1.18”     |
| Weight                    | 9±1g                                     |
| Supply Voltage            | 4.8V ~ 6.0V                              |
| Operating Voltage         | 3.5 - 6.0V                               |
| Stall Torque              | 1.2kg/cm (4.8V), 1.6kg/cm (6.0V)         |
| Working Speed             | 0.12sec/60 (4.8V no load)                |
| Dead Zone Width           | 5usec                                    |
| Neutral Location          | 1500us                                   |
| Operating Temperature     | -30°C to + 60°C                          |
| Rotation angle            | 360 degree <strong>(Continouos)</strong> |
| Cable Length              | 250mm                                    |

---

## Pin

| ![alt text](https://bit.ly/3dci7yo 'Servo motor pinout')         |
| ---------------------------------------------------------------- |
| Pinout of this servo motor is the same with standard servo motor |

| Pin                                       | Description   |
| ----------------------------------------- | ------------- |
| <span style="color: brown">Brown</span>   | GND(Negative) |
| <span style="color: red">Red</span>       | VCC(Positive) |
| <span style="color: orange">Orange</span> | PWM(Signal)   |

---

## Test

-   [Tutorial ](https://bit.ly/31BXdTL)

**to be updated**

--

## Troubleshooting

-   As above [descriptions](#descriptions), this servo does not have positional awareness and no hardware stop inside. Please see the [reference](#references) site below for understanding this servo.

-   when you test example code, you need to open the serial window and input a character as above.

**to be updated**

---

## Reference

-   Site:

    -   [https://www.arduino.cc/reference/en/language/functions/communication/serial/read](https://www.arduino.cc/reference/en/language/functions/communication/serial/read)

-   Test Video

        -   [Click to see the test video](https://bit.ly/39rG8jN)

        If you can't see the video on the google drive, plese click the 'open with Video Player for Google Drive' under the download menu.

**to be updated**

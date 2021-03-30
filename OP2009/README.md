# MG995 360 Degree Continuous Rotation Servo

## Table of Contents

-   [Descriptions](#descriptions)
-   [Specifications](#specifications)
-   [Components](#components)
-   [Testing](#Testing)
    -   [Connections](#connections)
    -   [Test Code](#test-code)
    -   [Troubleshooting](#troubleshooting)
-   [Reference](#reference)

---

## Descriptions (Important Information)

This factory modified version of the extremely common SG90 servo is a very basic continuous rotation servo. The servo offers an inexpensive and easy to control method of getting your small turret spinning or miniature robot moving. This servo can work with both 5 V and 3.3 V servo signals and has a standard servo connector.

The servo can be controlled using a direct connection to a single microcontroller I/O line without any additional electronics, which makes it a great miniature actuator for beginner robotics projects. Just drive it like a normal servo.

**Note:**

-   This servo has <strong>no positional awareness</strong> so that shaft can rotate freely.
-   You don't need to modify it yourself. It is factory modified.

---

## Specifications

| Features (Specifications)                        |                                        |
| ------------------------------------------------ | -------------------------------------- |
| Weight                                           | 55g                                    |
| Dimension                                        | 40.7 × 19.7 × 42.9 mm (LxWxH)          |
| Operating temperature                            | -30 ~ + 60 °                           |
| Deadband setting                                 | 4 microseconds                         |
| Rotation angle                                   | 360°                                   |
| Torque                                           | 4.8V: 130.5 oz-in (9.40 kg-cm)         |
|                                                  | 6.0V: 152.8 oz-in (11.00 kg-cm)        |
| Speed                                            | 4.8V: 0.20 sec/60°, 6.0V: 0.16 sec/60° |
| Servo type                                       | analog servo                           |
| Operation Voltage                                | 4.8 – 7.2Volts                         |
| Gear Type                                        | All Metal Gears                        |
| Stable and shockproof double ball bearing design |                                        |
| Control System                                   | Analog                                 |
| Cable Length: 250mm                              |                                        |

---

## Pin

| ![alt text](https://bit.ly/3uiYcF5 'Servo motor pinout')         |
| ---------------------------------------------------------------- |
| Pinout of this servo motor is the same with standard servo motor |

| Pin                                       | Description   |
| ----------------------------------------- | ------------- |
| <span style="color: brown">Brown</span>   | GND(Negative) |
| <span style="color: red">Red</span>       | VCC(Positive) |
| <span style="color: orange">Orange</span> | PWM(Signal)   |

## Test

-   [Tutorial Video](https://youtu.be/HnlKAwn6GG8)

**to be updated**

---

## Troubleshooting

-   As above [descriptions](#descriptions), this servo does not have positional awareness and no hardware stop inside. Please see the [reference](#references) site below for understanding this servo.

-   when you test example code, you need to open the serial window and input a character as above.

**to be updated**

---

## Reference

-   Site:

    -   [https://www.arduino.cc/reference/en/language/functions/communication/serial/read](https://www.arduino.cc/reference/en/language/functions/communication/serial/read)

-   Test Video with servo tester

    -   [Click to see the test video](https://bit.ly/3m4mVtI)

    If you can't see the video on the google drive, plese click the 'open with Video Player for Google Drive' under the download menu.

**to be updated**

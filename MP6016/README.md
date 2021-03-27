# TTP229 Capacitive Touch Sensor 16 Channel

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The TTP229 TonTouchTM IC is capacitive sensing design specifically for touch pad controls. The
device built in regulator for touch sensor. Stable sensing method can cover diversity conditions. Human
interfaces control panel links through non-conductive dielectric material. The main application is
focused at replacing of the mechanical switch or button. The ASSP can independently handle the 8
touch pads or up to 16 touch pads.

---

## Features (Specifications)

| Features (Specifications)                                                                     |
| --------------------------------------------------------------------------------------------- |
| Operating voltage：2.4V~5.5V for built-in regulator enable                                    |
| 2.0V~5.5V for built-in regulator disable                                                      |
| Built-in regulator with external enable/disable option                                        |
| Stand-by current                                                                              |
| At 3V, and sleep mode slow sampling rate 8Hz：                                                |
| Internal regulator is enabled, the Stand-by current                                           |
| => Typical 2.5uA for 16 input keys                                                            |
| => Typical 2.0uA for 8 input keys                                                             |
| Internal regulator is disabled, the Stand-by current                                          |
| => Typical 2.5uA for 16 input keys                                                            |
| => Typical 2.0uA for 8 input keys                                                             |
| Provides to set 8 direct keys or 16 direct keys by option                                     |
| Provides to set 8 separate outputs only for 8 direct input keys mode                          |
| Has two kinds of serial output interface, both can use for 8 and 16 direct input keys mode    |
| Include 2-wires serial interface and I2                                                       |
| C-bus slave interface, they are selected by option                                            |
| 8 separate outputs can select output driving types by option                                  |
| (CMOS/OD/OC with active high/low)                                                             |
| 2-wires serial interface can select active high or low by option                              |
| Offer multi-key or single-key feature by option                                               |
| Provides two kinds of sampling rate that slow sampling rate 8Hz                               |
| and fast sampling rate 64Hz at sleep mode                                                     |
| Have the maximum key-on time about 60sec by pin option                                        |
| Sensitivity can adjust by the capacitance(1~50pF) outside                                     |
| After power-on have about 0.5sec stable-time,                                                 |
| During the time do not touch the key pad, and all functions are disabled                      |
| Auto calibration for environment changing                                                     |
| And the re-calibration period is about 4.0sec, when all keys are not activated for fixed time |

---

## Pins

| **Pad No.** | **Pad Name** | **Share Pin** | **I/O Type** | **Pad Description**                                          |
| ----------- | ------------ | ------------- | ------------ | ------------------------------------------------------------ |
| 1           | TP15         | TPQ7          | I/O/OD       | Touch pad input pin(KEY-15)                                  |
|             |              |               |              | 8-keys direct output pin(TPQ7)                               |
| 2           | TP14         | TPQ6          | I/O/OD       | Touch pad input pin(KEY-14)                                  |
|             |              |               |              | 8-keys direct output pin(TPQ6)                               |
| 3           | SENADJ3      |               | I/O          | Touch pad TP12~15 sensitivity adjust common pin              |
| 4           | TP13         | TPQ5          | I/O/OD       | Touch pad input pin(KEY-13)                                  |
|             |              |               |              | 8-keys direct output pin(TPQ5)                               |
| 5           | TP12         | TPQ4          | I/O/OD       | Touch pad input pin(KEY-12)                                  |
|             |              |               |              | 8-keys direct output pin(TPQ4)                               |
| 6           | SDA          |               | I/OD         | Data pin for the I2C-bus serial data interface               |
| 7           | SDO          |               | O            | Data pin for the 2-wires serial output, option active        |
|             |              |               |              | Low/High by TP1                                              |
| 8           | SCL          |               | I            | Serial clock input pin for serial type                       |
|             |              |               |              | At 2-wires serial type can be set active Low/High by TP1     |
| 9           | SLPSENB      |               | I/O          | Sleep mode sensitivity adjustment pin for group-B(TP8~15)    |
| 10          | TP11         | TPQ3          | I/O/OD       | Touch pad input pin(KEY-11)                                  |
|             |              |               |              | 8-keys direct output pin(TPQ3)                               |
| 11          | TP10         | TPQ2          | I/O/OD       | Touch pad input pin(KEY-10)                                  |
|             |              |               |              | 8-keys direct output pin(TPQ2)                               |
| 12          | SENADJ2      |               | I/O          | Touch pad TP8~11 sensitivity adjust common pin               |
| 13          | TP9          | TPQ1          | I/O/OD       | Touch pad input pin(KEY-9)                                   |
|             |              |               |              | 8-keys direct output pin(TPQ1)                               |
| 14          | TP8          | TPQ0          | I/O/OD       | Touch pad input pin(KEY-8)                                   |
|             |              |               |              | 8-keys direct output pin(TPQ0)                               |
| 15          | TEST         |               | I-PL         | Only for test                                                |
| 16          | A2           |               | I-PH         | A2~0 are input pins for the I2C-bus device address selection |
| 17          | A1           |               | I-PH         | A2~0 are input pins for the I2C-bus device address selection |
| 18          | A0           |               | I-PH         | A2~0 are input pins for the I2C-bus device address selection |
| 19          | SLSERT       |               | I-PH         | The option pin for serial output type selection              |
|             |              |               |              | Default is 2-wires serial type                               |
| 20          | TP7          | SKSRT         | I/O          | Touch pad input pin(KEY-7)                                   |
|             |              |               |              | Maximum key-on time function option(Infinite/60sec)          |
|             |              |               |              | Default is infinite                                          |
| 21          | TP6          | SLWPTM        | I/O          | Touch pad input pin(KEY-6)                                   |
|             |              |               |              | Sleep mode sampling length function option(4.0/2.0mS)        |
|             |              |               |              | Default is 4.0ms                                             |
| 22          | SENADJ1      |               | I/O          | Touch pad TP4~7 sensitivity adjust common pin                |
| 23          | TP5          | WPSCT         | I/O          | Touch pad input pin(KEY-5)                                   |
|             |              |               |              | Sampling rate at sleep mode function option(8Hz/64Hz)        |
|             |              |               |              | Default is 8Hz                                               |
| 24          | TP4          | SKMS0         | I/O          | Touch pad input pin(KEY-4)                                   |
|             |              |               |              | Key action function option-0(Single-key/Multi-key)           |
|             |              |               |              | Default is all single-key                                    |
| 25          | VDD          |               | P            | Positive power supply                                        |
| 26          | VREG         |               | P            | Internal regulator output pin                                |
| 27          | ENSLP        |               | I-PH         | Sleep mode enable/disable function option                    |
|             |              |               |              | Default is enable                                            |
| 28          | VSS          |               | P            | Negative power supply, ground                                |
| 29          | REGEN        |               | I-PH         | Internal regulator enable/disable function option            |
|             |              |               |              | Default is enable                                            |
| 30          | SLPSENA      |               | I/O          | Sleep mode sensitivity adjustment pin for group-A(TP0~7)     |
| 31          | TP3          | SKMS1         | I/O          | Touch pad input pin(KEY-3)                                   |
|             |              |               |              | Key action function option-1(Single-key/Multi-key)           |
|             |              |               |              | Default is all single-key                                    |
| 32          | TP2          | KYSEL         | I/O          | Touch pad input pin(KEY-2)                                   |
|             |              |               |              | Key number function option(8-keys/16-keys)                   |
|             |              |               |              | Default is 8-keys                                            |
| 33          | SENADJ0      |               | I/O          | Touch pad TP0~3 sensitivity adjust common pin                |
| 34          | TP1          | SAHL          | I/O          | Touch pad input pin(KEY-1)                                   |
|             |              |               |              | utput type function option(Active High/Low)                  |
|             |              |               |              | Default is active-high for TPQ0~7,                           |
|             |              |               |              | active-low for 2-wires serial type(SCL and SDO)              |
| 35          | TP0          | OPDEN         | I/O          | Touch pad input pin(KEY-0)                                   |
|             |              |               |              | Output type function option(CMOS/OD/OC for 8-keys)           |
|             |              |               |              | Default is CMOS                                              |

| **Note：Pin Type**                                                                             |
| ---------------------------------------------------------------------------------------------- |
| I ＝＞ CMOS input only                                                                         |
| I-PH ＝＞ CMOS input and pull-high resister                                                    |
| I-PL ＝＞ CMOS input and pull-low resister                                                     |
| O ＝＞ CMOS push-pull output                                                                   |
| I/O ＝＞ CMOS I/O                                                                              |
| P ＝＞ Power / Ground                                                                          |
| OD ＝＞ CMOS open drain output                                                                 |
| (For OD TPQ0~TPQ7 pins have Diode protective circuit, SDA pin has no Diode protective circuit) |

---

## Test

-   [Tutorial I](https://bit.ly/3w661zi)
-   [Tutorial II](https://rdiot.tistory.com/134)
-   [Tutorial III](https://osoyoo.com/2016/07/11/capacitive-touchpad-16channel/)

-   [Tutorial Video I](https://youtu.be/2AEzQtKhBBY)
-   [Tutorial Video II](https://youtu.be/7W_DZgCuXPs)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [TTP229 Library](https://github.com/kiryanenko/TTP229)
-   [Article](https://bit.ly/39gybOA)
-   [TTP229 Datasheet](https://bit.ly/3tZf1Ey)

**to be updated..**

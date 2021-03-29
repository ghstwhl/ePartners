# NE555 Pulse Frequency Duty Cycle Adjustable Module (Signal generator, Timing module)

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The 555 timer IC is an integrated circuit that is popular used in a variety of timer, pulse generation, and oscillator applications. This NE555 frequency adjustable pulse generator Module utilizes the NE555 timer IC to generate pulses from about 4Hz to 1.3Khz, which can be used for experimental development, or driving a stepper motor, it would be also a good choice for users learning & experiencing the analog RC circuits.

---

## Features (Specifications)

| Features (Specifications)                                                                           |
| --------------------------------------------------------------------------------------------------- |
| Main chip: NE555                                                                                    |
| Input Voltage (VCC): 5V-15VDC                                                                       |
| Input current:>=100MA                                                                               |
| Output amplitude: 4.2V V-PP to 11.4V V-PP. (Varries with VCC voltage)                               |
| Maximum output current: 15MA (VCC=5V, V-PP greater than 50%), 35MA (VCC=12V, V-PP greater than 50%) |
| Output LED indicator (low level, LED is on, high level, LED is off; LED flashes with frequency      |
| The output frequency is continuously adjustable using the onboard jumpers and potentiometers.       |
| Jumper settings are seletable:                                                                      |
| LF file: 1Hz ~ 50Hz                                                                                 |
| IF file: 50Hz ~ 1kHz                                                                                |
| High-frequency file: 1KHz ~ 10kHz                                                                   |
| HF file: 10kHz ~ 200kHz                                                                             |
| The output duty cycle can fine-tuned using the onboard potentiometers.                              |
| Duty cycle and frequency are not separately adjustable;                                             |
| adjusting the duty cycle will change the frequency using the following variables:                   |
| Period T = 0.7 (RA +2 RB) C                                                                         |
| RA, RB are 0-10K Ohm adjustable potentiometers                                                      |
| 1Hz ~ 50Hz: C = 0.001UF                                                                             |
| 50Hz ~ 1kHz: C = 0.1UF                                                                              |
| 1KHz ~ 10kHz: C = 1UF                                                                               |
| 10kHz ~ 200kHz: C = 100UF                                                                           |
| Size: 31mm x 22mm                                                                                   |

---

## Pins

![alt text](https://bit.ly/2PzUlEu 'pinout')

| Pin Number | Description          |
| ---------- | -------------------- |
| GND        | Ground (-)           |
| VCC        | Power supply (+, 5V) |
| OUTPUT     | Signal Output        |

---

## Test

-   [Tutorial Video I](https://youtu.be/4pMszEbmnGA)
-   [Tutorial Video II](https://youtu.be/OyMLd5DYh6c)
-   [Tutorial Video III](https://youtu.be/lJmxjZwnb4Q)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [NE555 Datasheet](https://bit.ly/3syX3sh)

**to be updated..**

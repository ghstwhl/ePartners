# ATtiny85 USB Mini Development Board

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The ATtiny85 Microcontroller is possibly the smallest Microcontrollers available today. It is an 8-bit Microcontroller based on the AVR RISC Architecture. Physically, it needs only 8-pins for complete operation.

There are three variants of ATtiny85: ATtiny25, ATtiny45 and ATtiny85. The main difference between these three ICs is the amount of memory each device has (Flash, EEPROM and RAM).

ATtiny85 Microcontroller, the target device of this project has 8KB of In-system programmable Flash, 512B of EEPROM and 256B of SRAM.

---

## Features (Specifications)

| Features (Specifications)                        |
| ------------------------------------------------ |
| Support for the Arduino IDE 1.0+ (OSX/Win/Linux) |
| Power via USB or External Source                 |
| Onboard 5V Regulator                             |
| Built-in USB                                     |
| 6 I/O Pins                                       |
| 8k Flash Memory (about 6k after bootloader)      |
| I2C and SPI (vis USI)                            |
| PWM on 3 pins (more possible with Software PWM)  |
| ADC on 4 pins                                    |
| Power LED and Test/Status LED                    |

---

## Pins

| ![alt text](https://bit.ly/31VDw9M 'ATtiny85') |
| ---------------------------------------------- |

| Pin no. | Pin Name                                | Description   | Secondary Function                                         |
| ------- | --------------------------------------- | ------------- | ---------------------------------------------------------- |
| 1       | PB5 (PCINT5/ADC0/dW)                    | Pin5 of PORTB | PCINT5 : Pin Change Interrupt 0, Source5                   |
|         |                                         |               | RESET : Reset Pin                                          |
|         |                                         |               | ADC0 : ADC Input Channel 0                                 |
|         |                                         |               | dW : debug WIRE I/O                                        |
| 2       | PB3 (PCINT3/XTAL1/CLKI/ADC3)            | Pin3 of PORTB | PCINT3 : Pin Change Interrupt 0, Source3                   |
|         |                                         |               | XTAL1 : Crystal Oscillator Pin1                            |
|         |                                         |               | CLKI : External Clock Input                                |
|         |                                         |               | OC1B : Complementary Timer/Counter1 Compare Match B Output |
|         |                                         |               | ADC3 : ADC Input Channel 3                                 |
| 3       | PB4 (PCINT4/XTAL2/CLKO/OC1B/ADC2)       | Pin4 of PORTB | PCINT4 : Pin Change Interrupt 0, Source 4                  |
|         |                                         |               | XTAL2 : Crystal Oscillator Pin 2                           |
|         |                                         |               | CLKO : System Clock Output                                 |
|         |                                         |               | OC1B: Timer/Counter1 Compare Match B Output                |
|         |                                         |               | ADC2 : ADC Input Channel 2                                 |
| 4       | GND                                     |               | Connected to Ground                                        |
| 5       | PB0(MOSI/DI/SDA/AIN0/OC0A/AREF/ PCINT0) | Pin0 of PORTB | MOSI : SPI Master Data Output / Slave Data Input           |
|         |                                         |               | DI : USI Data Input (Three Wire Mode)                      |
|         |                                         |               | SDA : USI Data Input (Two Wire Mode)                       |
|         |                                         |               | AIN0 : Analog Comparator, Positive Input                   |
|         |                                         |               | OC0A : Timer/Counter0 Compare Match A output               |
|         |                                         |               | : Complementary Timer/Counter1 Compare Match A Output      |
|         |                                         |               | AREF : External Analog Reference                           |
|         |                                         |               | PCINT0 : Pin Change Interrupt 0, Source 0                  |
| 6       | PB1(MISO/D0/AIN1/OC0B/OC1A/ PCINT1)     | Pin1 of PORTB | MISO : SPI Master Data Input / Slave Data Output           |
|         |                                         |               | DO : USI Data Output (Three Wire Mode)                     |
|         |                                         |               | AIN1 : Analog Comparator, Negative Input                   |
|         |                                         |               | OC0B : Timer/Counter0 Compare Match B Output               |
|         |                                         |               | OC1A: Timer/Counter1 Compare Match A Output                |
|         |                                         |               | PCINT1 : Pin Change Interrupt 0, Source 1                  |
| 7       | PB2(SCK/USCK/SCL/ADC1/T0/INT0/ PCINT2)  | Pin2 of PORTB | SCK : Serial Clock Input                                   |
|         |                                         |               | USCK : USI Clock (Three Wire Mode)                         |
|         |                                         |               | SCL : USI Clock (Two Wire Mode)                            |
|         |                                         |               | ADC1 : ADC Input Channel 1                                 |
|         |                                         |               | T0 : Timer/Counter0 Clock Source                           |
|         |                                         |               | INT0 : External Interrupt 0 Input                          |
|         |                                         |               | PCINT2 : Pin Change Interrupt 0, Source 2                  |
| 8       | VCC                                     |               | Connected to positive voltage                              |

---

## Test

-   [Tutorial I](https://bit.ly/ATtiny81-docs)
-   [Tutorial II](http://bit.ly/ATtiny85-USB-Mini)
-   [Tutorial III](https://bit.ly/3dLOHr7)

-   [Tutorial Video I](https://youtu.be/fOBGdSYi318)
-   [Tutorial Video II](https://youtu.be/MmDBvgrYGZs)
-   [Tutorial Video III](https://youtu.be/KroH7rAdbWE)

**to be updated..**

---

## Troubleshooting

**to be updated..**

---

## References

-   [ATtiny85 Datasheet](https://bit.ly/39UzvH7)

**to be updated..**

# MG995 360 Degree Continuous Rotation Servo

## Table of Contents
- [Descriptions](#descriptions)
- [Specifications](#specifications)
- [Components](#components)
- [Testing](#Testing)
  - [Connections](#connections)
  - [Test Code](#test-code)
  - [Troubleshooting](#troubleshooting)
- [Reference](#reference)
    
---

## Descriptions (Important Information)
This servo motor's operation is more similar to an ordinary DC motor than a standard servo motor which means <strong>this servo has no positional awareness so that shaft can rotate freely.</strong>
And this servo motor does not require additional motor drivers and is plug and play. Please see the following example code.

![alt text](Pictures/MG995.jpg "MG995 Servo")

## Specifications
- Weight: 55g
- Dimension : 40.7 × 19.7 × 42.9 mm (LxWxH)
- Operating temperature: -30 ~ + 60 °
- Deadband setting: 4 microseconds
- Rotation angle: 360°
- Torque: 4.8V: 130.5 oz-in (9.40 kg-cm), 6.0V: 152.8 oz-in (11.00 kg-cm)
- Speed: 4.8V: 0.20 sec/60°, 6.0V: 0.16 sec/60°
- Servo type: analog servo
- Operation Voltage : 4.8 – 7.2Volts
- Gear Type: All Metal Gears
- Stable and shockproof double ball bearing design
- Control System: Analog

- Interface Description:
- <span style="color: brown">Brown</span>: GND(Negative)
- <span style="color: red">Red</span>: VCC(Positive)
- <span style="color: orange">Orange</span>: PWM(Signal)
- Cable Length: 250mm

## Component
* Please click the link with 'Ctrl' key or 'CMD' key, if you would like to open the link in a new tab!

- [Servo MG995 360 Degree Continuous Rotation](https://www.trademe.co.nz/electronics-photography/other-electronics/electronic-components/other/listing-2688202015.htm?rsqid=a744f81d390d4678a35508be78b9c7c0-001)
- [Servo Tester](https://www.trademe.co.nz/electronics-photography/other-electronics/electronic-components/other/listing-2684098940.htm?rsqid=27fbf7bfa7fb47b4b44ffd008cdda51e-001)
- [Arduino Uno R3 MEGA328P CH340](https://www.trademe.co.nz/electronics-photography/other-electronics/electronic-components/other/listing-2651898157.htm?rsqid=929e0e9ffa584c05a4e74094cd4b87c6-004/)

---

## Testing

## Connections
### Interface Description:
- <span style="color: brown">Brown</span>: GND(Negative)
- <span style="color: red">Red</span>: VCC(Positive)
- <span style="color: orange">Orange</span>: PWM(Signal)

| ![alt text](Pictures/servo.png "Servo motor pinout") |
| -- |
| Pinout of this servo motor is the same with standard servo motor |

## Test Code
* This example needs just standard servo library on Arduino IDE.

```c++
#include <Servo.h> // Include standard servo library

Servo myservo;  // create servo object to control a servo

char incomingChar; // for incoming serial data

void setup() {
  Serial.begin(9600); // opens serial port, sets data rate to 9600 bps
  myservo.attach(6); // connect servo motor to the pin 6 of Arduino board
}

void loop() {
  // send data only when you receive data:
  if (Serial.available() > 0) {
    // read the incoming byte:
    incomingChar = Serial.read();

    if(incomingChar == 'w') {
      myservo.writeMicroseconds(700); // to rotate to the clockwise
      Serial.println("Clockwise");
    }
    else if(incomingChar == 's') { // to stop rotating
      myservo.writeMicroseconds(1500);
      Serial.println("Stop");
    }
    else if(incomingChar == 'c') { // to rotate to the counterclockwise
      myservo.writeMicroseconds(2300);
      Serial.println("CounterClockWise");
    }
  }
}


```

## Troubleshooting
- As above [descriptions](#descriptions), this servo does not have positional awareness and no hardware stop inside. Please see the [reference](#references) site below for understanding this servo.

- when you test example code, you need to open the serial window and input a character as above.

## Reference
- Site:
  - [https://www.arduino.cc/reference/en/language/functions/communication/serial/read](https://www.arduino.cc/reference/en/language/functions/communication/serial/read)

- Test Video with servo tester
  - [Click to see the test video](https://drive.google.com/file/d/1iC_SUgOe_RWc-1voNUQhlDNEl39CSWug/view?usp=sharing)

  If you can't see the video on the google drive, plese click the 'open with Video Player for Google Drive' under the download menu.

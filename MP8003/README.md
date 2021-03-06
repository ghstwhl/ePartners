# Mini MP3 Player Module TF Card U Disk Audio Voice Module Board

## Table of Contents

-   [Descriptions](#descriptions)
-   [Features](#features)
-   [Pins](#pins)
-   [Test](#test-code)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Descriptions

The DFPlayer Mini MP3 Player For Arduino is a small and low price MP3 module with an simplified output directly to the speaker. The module can be used as a stand alone module with attached battery, speaker and push buttons or used in combination with an Arduino UNO or any other with RX/TX capabilities.

---

## Features (Specifications)

| Features (Specifications)                                                                      |
| ---------------------------------------------------------------------------------------------- |
| Supported sampling rates (kHz): 8/11.025/12/16/22.05/24/32/44.1/48                             |
| 24 -bit DAC output, support for dynamic range 90dB , SNR support 85dB                          |
| Fully supports FAT16 , FAT32 file system                                                       |
| Maximum support 32G of the TF card, support 32G of U disk, 64M bytes NORFLASH                  |
| A variety of control modes, I/O control mode, serial mode, AD button control mode              |
| Advertising sound waiting function, the music can be suspended.                                |
| When advertising is over in the music continue to play                                         |
| Audio data sorted by folder, supports up to 100 folders, every folder can hold up to 255 songs |
| 30 level adjustable volume, 6 -level EQ adjustable                                             |

---

## Pins

![alt text](https://bit.ly/3d5plEk)

| No. | Pin Number | Description                | Note                              |
| --- | ---------- | -------------------------- | --------------------------------- |
| 1   | VCC        | Input Voltage              | DC3.2~5.0V;Type:DC4.2V            |
| 2   | RX         | UART serial input          |                                   |
| 3   | TX         | UART serial output         |                                   |
| 4   | DAC_R      | Audio output right channel | Drive earphone and amplifier      |
| 5   | DAC_L      | Audio output left channel  | Drive earphone and amplifier      |
| 6   | SPK        | Speaker -                  | Drive apeaker less than 3W        |
| 7   | GND        | Ground                     | Power GND                         |
| 8   | SPK_1      | Speaker +                  | Drive speaker less than 3W        |
| 9   | IO_1       | Trigger port_1             | Short press to play previous      |
|     |            |                            | (long press to decrease volume)   |
| 10  | GND        | Ground                     | Power GND                         |
| 11  | IO_2       | Trigger port_2             | Short press to play next          |
|     |            |                            | (long press to increase volume)   |
| 12  | ADKEY_1    | AD Port_1                  | Trigger play first segment        |
| 13  | ADKEY_2    | AD Port_2                  | Trigger play fifth segment        |
| 14  | USB+       | USB+ DP                    | USB Port                          |
| 15  | USB-       | USB- DM                    | USB Port                          |
| 16  | BUSY       | Playing Status             | Low means playing / High means no |

---

## Test

-   [Tutorial I](https://www.instructables.com/MP3-Player-With-Arduino-Using-DF-Player-Mini/)
-   [Tutorial II](https://maker.pro/arduino/projects/how-to-use-the-dfmini-player-mp3-module-with-arduino)
-   [Tutorial III](https://wiki.dfrobot.com/DFPlayer_Mini_SKU_DFR0299)

-   [Tutorial Video I](https://youtu.be/gMv2xGHLXdU)
-   [Tutorial Video II](https://youtu.be/UodfePdNfg8)
-   [Tutorial Video III](https://youtu.be/P42ICrgAtS4)

-   **to be updated..**

---

## Troubleshooting
- If you fail to play the file & adjust the volume, please try the below code.
- It's tested with a file (Not multiple files)

```c++
#include "Arduino.h"
#include "SoftwareSerial.h"
#include "DFRobotDFPlayerMini.h"

#define VOLUME             15   // Set volume value. From 0 to 30
#define MAX_VOLUME_LEVEL   30

//#define SERIAL_DEBUG

SoftwareSerial mySoftwareSerial(10, 11); // RX, TX
DFRobotDFPlayerMini myDFPlayer;
void printDetail(uint8_t type, int value);
int setVolume(int vol);

void setup()
{
  mySoftwareSerial.begin(9600);
#ifdef SERIAL_DEBUG
  Serial.begin(115200);


  Serial.println();
  Serial.println(F("DFRobot DFPlayer Mini Demo"));
  Serial.println(F("Initializing DFPlayer ... (May take 3~5 seconds)"));
#endif

  if (!myDFPlayer.begin(mySoftwareSerial)) {  //Use softwareSerial to communicate with mp3.
#ifdef SERIAL_DEBUG
    Serial.println(F("Unable to begin:"));
    Serial.println(F("1.Please recheck the connection!"));
    Serial.println(F("2.Please insert the SD card!"));
#endif
    while (true) {
      delay(0); // Code to compatible with ESP8266 watch dog.
    }
  }

#ifdef SERIAL_DEBUG
  Serial.println(F("DFPlayer Mini online."));
#endif

  setVolume(VOLUME);

//  myDFPlayer.play(1); 
  myDFPlayer.next(); 
}

void loop() {}

int setVolume(int vol) {
  myDFPlayer.volume(0);

  for (int i = 0; i < vol; i++) {
    myDFPlayer.volumeUp();
  }
}
```


**to be updated..**

---

## References

-   [Manual](https://bit.ly/3dqlIsX)

**to be updated..**

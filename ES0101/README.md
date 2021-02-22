# ESP-01s Tutorial (Wifi Connection)

## Table of Contents

-   [Description](#description)
-   [Features](#features)
-   [Pin Decription](#pin-description)
-   [Schematic](#schematic)
-   [Tutorials](#tutorials)
    -   [Test-environment](#test-environment)
        -   [Hardware](#hardware)
        -   [Software](#software)
    -   [Test](#test)
        -   [Test Code](#test-code)
        -   [Test Result](#test-result)
-   [Troubleshooting for Windows](#troubleshooting-for-windows)
-   [References](#references)

---

## Description

ESP-01 WiFi module is developed by
encapsulates Tensilica L106 integrates industry
Clock speed support 80 MHz, 160 MHz, supports the RTOS, integrated Wi
The module supports standard IEEE802.11
add modules to an existing device networking, or building a separate network controller.
ESP8266 is high integration wireless SOCs, designed for space and power constrained mobile platform
It provides unsurpassed ability to embed Wi
application, with the lowest cost, and minimal space requirement.

---

## Feature

| Features                                                                                   |
| ------------------------------------------------------------------------------------------ |
| 802.11 b/g/n                                                                               |
| Integrated low power 32-bit MCU                                                            |
| Integrated 10-bit ADC                                                                      |
| Integrated TCP/IP protocol stack                                                           |
| Integrated TR switch, balun, LNA, power amplifier and matching network                     |
| Integrated PLL, regulators, and power management units                                     |
| Supports antenna diversity                                                                 |
| Wi-Fi 2.4 GHz, support WPA/WPA2                                                            |
| Support STA/AP/STA+AP operation modes                                                      |
| Support Smart Link Function for both Android and iOS devices                               |
| SDIO 2.0, (H) SPI, UART, I2C, I2S, IRDA, PWM, GPIO                                         |
| STBC, 1x1 MIMO, 2x1 MIMO                                                                   |
| A-MPDU & A-MSDU aggregation and 0.4s guard interval                                        |
| Deep sleep power <10uA, Power down leakage current < 5uA                                   |
| Wake up and transmit packets in < 2ms                                                      |
| Standby power consumption of < 1.0mW (DTIM3)                                               |
| +20dBm output power in 802.11b mode                                                        |
| Operating temperature range -40C ~ 125C                                                    |
| 1MB Flash Memory                                                                           |
| Can be used as Station or Access Point or both combined                                    |
| Supports serial communication hence compatible with many development platform like Arduino |
| Can be programmed using Arduino IDE or AT-commands or Lua Script                           |

---

## Pin Description

| NO. | Pin Name | Alternate Name | Normally used for                                      |
| --- | -------- | -------------- | ------------------------------------------------------ |
| 1   | GND      | -              | Connected to the ground of the circuit                 |
| 2   | TX       | GPIO-1         | Connected to RX pin of programmer/uC to upload program |
| 3   | GPIO-2   | -              | General purpose Input/Output pin                       |
| 4   | CH_EN    | -              | Chip Enable - Active high                              |
| 5   | GPIO-0   | Flash          | General purpose Input/Output pin                       |
| 6   | Reset    | -              | Resets the module                                      |
| 7   | RX       | GPIO-3         | General purpose Input/Output pin                       |
| 8   | VCC      | -              | Connect to +3.3V only                                  |

---

## Schematic

| ![alt text](https://bit.ly/3dAbJ5W 'ESP01-S') |
| --------------------------------------------- |

---

---

## Tutorials

### Install the Add-on to the Arduino IDE

| Installing ESP8266 Add-on to Arduino IDE      |
| :-------------------------------------------- |
| ![alt text](https://bit.ly/3aG93BV 'ESP8266') |
| ![alt text](https://bit.ly/2ZzqopM 'ESP8266') |
| ![alt text](https://bit.ly/2P1ZViz 'ESP8266') |

```c++
#include <ESP8266WiFi.h>

const char* ssid = "Type your WIFI ssid";//type your ssid
const char* password = "Type your WIFI password";//type your password

int ledPin_0 = 0;
int ledPin_1 = 2; // GPIO2 of ESP8266
WiFiServer server(80);

void setup() {
  Serial.begin(115200);
  delay(10);

  pinMode(ledPin_0, OUTPUT);
  pinMode(ledPin_1, OUTPUT);
  digitalWrite(ledPin_0, LOW);
  digitalWrite(ledPin_1, LOW);

  // Connect to WiFi network
  Serial.println();
  Serial.println();
  Serial.print("Connecting to ");
  Serial.println(ssid);

  WiFi.begin(ssid, password);

  while (WiFi.status() != WL_CONNECTED) {
    delay(500);
    Serial.print(".");
  }
  Serial.println("");
  Serial.println("WiFi connected");

  // Start the server
  server.begin();
  Serial.println("Server started");

  // Print the IP address
  Serial.print("Use this URL to connect: ");
  Serial.print("http://");
  Serial.print(WiFi.localIP());
  Serial.println("/");

}

void loop() {
  // Check if a client has connected
  WiFiClient client = server.available();
  if (!client) {
    return;
  }

  // Wait until the client sends some data
  Serial.println("new client");
  while(!client.available()){
    delay(1);
  }

  // Read the first line of the request
  String request = client.readStringUntil('\r');
  Serial.println(request);
  client.flush();

  // Match the request

  int value = LOW;
  if (request.indexOf("/LED=ON") != -1) {
    digitalWrite(ledPin_0, LOW);
    digitalWrite(ledPin_1, HIGH);
    value = HIGH;
  }
  if (request.indexOf("/LED=OFF") != -1){
    digitalWrite(ledPin_0, HIGH);
    digitalWrite(ledPin_1, LOW);
    value = LOW;
  }

// Set ledPin according to the request
//digitalWrite(ledPin, value);


  // Return the response
  client.println("HTTP/1.1 200 OK");
  client.println("Content-Type: text/html");
  client.println(""); //  do not forget this one
  client.println("<!DOCTYPE HTML>");
  client.println("<html>");

  client.print("Led pin is now: ");

  if(value == HIGH) {
    client.print("On");
  } else {
    client.print("Off");
  }
  client.println("<br><br>");
  client.println("Click <a href=\"/LED=ON\">here</a> turn the LED on pin 0 or 2 ON<br>");
  client.println("Click <a href=\"/LED=OFF\">here</a> turn the LED on pin 0 or 2 OFF<br>");
  client.println("</html>");

  delay(1);
  Serial.println("Client disonnected");
  Serial.println("");

}
```

---

## Test result

| ![alt text](Pictures/Connection_3.JPG 'test_result')                                                                   |
| ---------------------------------------------------------------------------------------------------------------------- |
| [Click here to see the test Video](https://drive.google.com/file/d/1Kh5V_BQc-Tqt1xwRKg5C1WmTdZHwsH0Q/view?usp=sharing) |

| Red wire    | 3.3V                   |
| ----------- | ---------------------- |
| Grey wire   | ESP-01 RX -> PL2303 TX |
| Yellow wire | ESP-01 TX -> PL2303 RX |
| Black wire  | GND                    |
| Green wire  | GPIO2 -> Green LED     |
| White wire  | GPIO0 -> White LED     |

---

## Troubleshooting

| 1. Installing ESP8266 Add-on to Arduino IDE   |
| :-------------------------------------------- |
| ![alt text](Pictures/ESP8266_1.png 'ESP8266') |
| ![alt text](Pictures/ESP8266_2.png 'ESP8266') |
| ![alt text](Pictures/ESP8266_3.png 'ESP8266') |

| 2. If you cannot upload the code, check your COM port in the <b>Device manager</b>. |
| :---------------------------------------------------------------------------------- |
| ![alt text](Pictures/check_port.png 'COM port')                                     |

3. EN pin (or CHPD pin) must be connected to 3.3V
4. Before the code is upload to ESP-01s, GPIO 0 pin must be connected to GND.
5. After uploading the code, GPIO 0 pin must be disconnected from GND.

---

## References

-   Datasheet
    -   [ESP-01(s)]http://www.microchip.ua/wireless/esp01.pdf
    -   [PL2303 USB to TTL Adapter](https://www.mpja.com/download/pl2303hxreva_v1.6.pdf)

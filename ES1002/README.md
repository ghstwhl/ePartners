# ESP8266 ESP-12E NodeMcu V3 with CH340

## Table of Contents

-   [Description](#description)
-   [Features](#features)
-   [Pinout](#pinout)
-   [Tutorials](#tutorials)
    -   [Test-environment](#test-environment)
        -   [Hardware](#hardware)
        -   [Software](#software)
    -   [Test](#test) **..Coming soon..**
        -   [Test Code](#test-code) **..Coming soon..**
        -   [Test Result](#test-result) **..Coming soon..**
-   [Troubleshooting](#troubleshooting) **..Coming soon..**
-   [References](#references) **..Coming soon..**

---

## Description

-   NodeMCU has ESP-12 based serial WiFi integrated on board to provide GPIO, PWM, ADC, I2C and 1-WIRE resources at your finger tips, built-in USB-TTL serial with super reliable industrial strength CH340 for superior stability on all supported platforms.

-   ESP8266 is a highly integrated chip designed for the needs of a new connected world.

-   It offers a complete and self-contained Wi-Fi networking solution, allowing it to either host the application or to offload all Wi-Fi networking functions from another application processor.

-   ESP8266 has powerful on-board processing and storage capabilities that allow it to be integrated with the sensors and other application specific devices through its GPIOs with minimal development up-front and minimal loading during run-time.

---

## Features

| Features                |                 |
| ----------------------- | --------------- |
| Microcontroller         | ESP-8266 32-Bit |
| Operating Voltage       | 3.3V            |
| Input Voltage           | 4.5V-10V        |
| Digital I/O Pins (DIO)  | 11 Pins         |
| Analog Input Pins (ADC) | 1 Pin           |
| ADC Range               | 0-3.3V          |
| UART                    | 1               |
| SPI                     | 1               |
| I2C                     | 1               |
| Flash Memory            | 4MB             |
| SRAM                    | 64KB            |
| Clock Speed             | 80 MHz          |
| USB-TTL                 | CH340G          |
| USB Connector           | Micro USB       |
| Antenna                 | PCB Antenna     |
| Size                    | 58 \* 32mm      |

---

## Pinout

![alt text](https://bit.ly/3pS7HZd 'ESP8266 NodeMCU')

---

## Tutorials

### Test Environment

#### Harware

| ![alt text](https://bit.ly/3bDAyLw 'ESP8266 NodeMCU') | ![alt text](https://bit.ly/3dHKR3Z 'Micro USB cable') |
| ----------------------------------------------------- | ----------------------------------------------------- |
| ESP8266 NodeMCU                                       | Micro USB Cable                                       |

---

#### Software https://bit.ly/3sqeo6s

-   **Setup for using NodeMCU on Arduino IDE**

    | ![alt text](https://bit.ly/3sqeo6s 'ESP8266 NodeMCU') | ![alt text](https://bit.ly/3aQAjO3 'ESP8266 NodeMCU') | ![alt text](https://bit.ly/37GNDCv 'ESP8266 NodeMCU') |
    | ----------------------------------------------------- | ----------------------------------------------------- | ----------------------------------------------------- |
    | ![alt text](https://bit.ly/2P4dmOR 'ESP8266 NodeMCU') | ![alt text](https://bit.ly/3qSn8So 'ESP8266 NodeMCU') | ![alt text](https://bit.ly/2ZLBVT5 'ESP8266 NodeMCU') |
    | ![alt text](https://bit.ly/3spBg5X 'ESP8266 NodeMCU') |

-   **Add a library for testing**

**Firstly, download the library [here](libraries/)**

| ![alt text](https://bit.ly/3aRl2N5 'ESP8266 NodeMCU') | ![alt text](https://bit.ly/3pRTU4K 'ESP8266 NodeMCU') | ![alt text](https://bit.ly/37IfGSo 'ESP8266 NodeMCU') |
| ----------------------------------------------------- | ----------------------------------------------------- | ----------------------------------------------------- |
| Select "Add a library"                                | Find your download folder                             | Type "#include<ESP8266WiFi.h>"                        |

---

### Test

#### Test Code

```c++
#include <ESP8266WiFi.h> // "ESP8266WiFi" should be red, if it is black, something's wrong.

const char* ssid = "type your ssid";//type your ssid
const char* password = "type your password";//type your password

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
  client.println("Click <a href=\"/LED=ON\">here</a> turn the LED on pin 2 ON<br>");
  client.println("Click <a href=\"/LED=OFF\">here</a> turn the LED on pin 2 OFF<br>");
  client.println("</html>");

  delay(1);
  Serial.println("Client disonnected");
  Serial.println("");

}

```

---

#### Test Result (Comming soon..)

**Temporary**

| ![alt text](https://bit.ly/37IY60m 'ESP8266 NodeMCU') |
| ----------------------------------------------------- |
| ![alt text](https://bit.ly/37MCQH5 'ESP8266 NodeMCU') |

## References

-   [ESP8266 Official](https://www.espressif.com/en/products/modules/esp8266)
-   [NodeMCU Docs](https://nodemcu.readthedocs.io/en/release/)
-   [Tutorial Video](https://youtu.be/G6CqvhXpBKM)
-   [Tutorial Guide](https://www.instructables.com/Get-Started-with-ESP8266-Using-AT-Commands-NodeMCU/)

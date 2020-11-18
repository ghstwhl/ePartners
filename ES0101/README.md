# ESP-01s Tutorial (Wifi Connection)

## Table of Contents

-   [Intro](#intro)
-   [Component](#component)
-   [Connections](#connections)
-   [Test Code](#test-code)
    -   [Test result](#test-result)
-   [Troubleshooting](#troubleshooting)
-   [References](#references)

---

## Intro

This is ESP01-s tutorial with connection and simple working test.
The test includes connection to WIFI and controlling 2 LEDs.

This page will be updated soon.

---

## Component

-   Please click the link with 'Ctrl' key or 'CMD' key, if you would like to open the link in a new tab!

| ![alt text](Pictures/ES0102.png 'ESP-01s')                                          |
| ----------------------------------------------------------------------------------- |
| [ESP-01s](https://www.trademe.co.nz/Browse/Listing.aspx?id=2741117322&bof=Vpo9gmFT) |

| ![alt text](Pictures/SC0003.png 'PL2303') |
| ----------------------------------------- |


[PL2303 USB to TTL Adapter](https://www.trademe.co.nz/Browse/Listing.aspx?id=2746950880&bof=BF6PYkto)

| ![alt text](Pictures/NP1022.png '5mm LED Green') |
| ------------------------------------------------ |


[5mm LED Green](https://www.trademe.co.nz/Browse/Listing.aspx?id=2746946823&bof=PelvUgYY)

| ![alt text](Pictures/NP1025.png '5mm LED White') |
| ------------------------------------------------ |


[5mm LED White](https://www.trademe.co.nz/Browse/Listing.aspx?id=2746946645&bof=Jup8NVFL)

| ![alt text](Pictures/RS2721.png 'Resistor - 200 Ohm') |
| ----------------------------------------------------- |


[Resistor - 200 Ohm](https://www.trademe.co.nz/Browse/Listing.aspx?id=2743360863&bof=Q9u7yWWy)

| ![alt text](Pictures/BB1005.png 'Breadboard') |
| --------------------------------------------- |


[Breadboard](https://www.trademe.co.nz/Browse/Listing.aspx?id=2746168815&bof=VpNbpqcQ)

---

## Connections

| ESP-01s | PL2303 | LEDs        |
| ------- | ------ | ----------- |
| 3.3V    | 3.3V   |             |
| RX      | TX     |             |
| TX      | RX     |             |
| GND     | GND    | GND         |
| GPIO2   |        | Green LED + |
| GPIO0   |        | White LED + |

| After updating the code, you will see follows. |
| ---------------------------------------------- |
| ![alt text](Pictures/get_ip.png 'getip')       |
| ![alt text](Pictures/web_page.png 'webpage')   |

---

## Test Code

-   To test the following example with Arduino IDE, you need to install the ESP8266 add-on. If you haven't installed the ESP8266 add-on, please follow the troubleshooting section.

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

| 2. If you cannot upload the code, check you COM port in the <b>Device manager</b>. |
| :--------------------------------------------------------------------------------- |
| ![alt text](Pictures/check_port.png 'COM port')                                    |

3. EN pin (or CHPD pin) must be connected to 3.3V
4. Before the code is upload to ESP-01s, GPIO 0 pin must be connected to GND.
5. After uploading the code, GPIO 0 pin must be disconnected from GND.

---

## References

-   Datasheet
    -   [ESP-01(s)]http://www.microchip.ua/wireless/esp01.pdf
    -   [PL2303 USB to TTL Adapter](https://www.mpja.com/download/pl2303hxreva_v1.6.pdf)

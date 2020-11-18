# LCD 2004 3.3V Green

This is the test note of 2004 LCD 3.3V with I2C adater and Arduino Uno. You may need a [library](Library/) for the I2C adapter.

## Table of Contents
- [Component](#component)
- [With I2C LCD Adapter](#with-i2c-lcd-adapter)
  - [Connections](#connections)
  - [Test Code](#test-code)
  - [Troubleshooting](#troubleshooting)
- [Without I2C LCD Adapter](#without-i2c-lcd-adapter)
  - [Test Code](#test-code-1)
- [References](#references)
    
---

## Component
* Please click the link with 'Ctrl' key or 'CMD' key, if you would like to open the link in a new tab!

- [LCD 2004 3.3V Green](https://www.trademe.co.nz/electronics-photography/other-electronics/electronic-components/other/listing-2658798410.htm?rsqid=99c284d3dcd44811b0acc3daaf7acd21-005)
- [I2C LCD Adapter Plate](https://www.trademe.co.nz/electronics-photography/other-electronics/electronic-components/other/listing-2657940961.htm?rsqid=3915eefe3ba5453ca671aa0b010a3fbc-001)
- [Arduino Uno R3 MEGA328P CH340](https://www.trademe.co.nz/electronics-photography/other-electronics/electronic-components/other/listing-2651898157.htm?rsqid=929e0e9ffa584c05a4e74094cd4b87c6-004)

## With I2C LCD Adapter

## Connections
- Connect SDA, SCL, <b>VCC(3.3V on Arduino board)</b>, GND pins of I2C Adapter to the same each pin of Arduino board

## Test Code
* This example is included in the [library](Library/) folder.

```c++
//Compatible with the Arduino IDE 1.0
//Library version:1.1

#include <Wire.h> 
#include <LiquidCrystal_I2C.h>

// set the LCD address to 0x27 for a 16 chars and 2 line display
LiquidCrystal_I2C lcd(0x27, 20, 4);  

void setup()
{
  lcd.init();                      // initialize the lcd 
  // Print a message to the LCD.
  lcd.backlight();

  // first 0 is cursor position, second 0 is line position
  lcd.setCursor ( 0, 0 );             // go to the top left corner
  lcd.print("    Hello,world!    ");  // write this string on the top row
  lcd.setCursor ( 0, 1 );             // go to the 2nd row
  lcd.print("Happy Coding!");  // pad string with spaces for centering
  lcd.setCursor ( 0, 2 );             // go to the third row
  lcd.print("Enjoy your life!");  // pad with spaces for centering
  lcd.setCursor ( 0, 3 );             // go to the fourth row
  lcd.print("Tested by ePartners!");
}


void loop()
{
  
}
```



## Troubleshooting

<strong>1. I2C Scanner Code</strong> : You may need to scan the I2C device address with below code

```c++
#include <Wire.h> 

void setup()
{
  Wire.begin();

  Serial.begin(9600);
  while (!Serial);             //  wait for serial monitor
  Serial.println("\nI2C Scanner");
}


void loop()
{
  byte error, address;
  int nDevices;

  Serial.println("Scanning...");

  nDevices = 0;
  for(address = 1; address < 127; address++ )
  {
    // The i2c_scanner uses the return value of
    // the Write.endTransmisstion to see if
    // a device did acknowledge to the address.
    Wire.beginTransmission(address);
    error = Wire.endTransmission();

    if (error == 0)
    {
      Serial.print("I2C device found at address 0x");
      if (address<16)
        Serial.print("0");
      Serial.print(address,HEX);
      Serial.println("  !");

      nDevices++;
    }
    else if (error==4)
    {
      Serial.print("Unknown error at address 0x");
      if (address<16)
        Serial.print("0");
      Serial.println(address,HEX);
    }    
  }
  if (nDevices == 0)
    Serial.println("No I2C devices found\n");
  else
    Serial.println("done\n");

  delay(5000);           // wait 5 seconds for next scan
}
```


<strong>2. SDA & SCL Pins on Arduino Uno board</strong>
  - 16U2 board: 
    - Pin A4 = SDA(I2C)
    - Pin A5 = SCL(I2C)
    - Check out the pinout here (https://bit.ly/2UxduWZ)

  - CH340 board: You can find those pins on the line of digital pins
    - Check out the pinout here (https://bit.ly/2AUk5Ee)

<strong>3. Adjust the backlight by the potentiometer of I2C LCD Adapter</strong>
  
  | ![alt text](Pictures/2004.jpg "Turn the potentiometer") |
  | -- |
  | If you can't see any charaters on the LCD, adjust the contrast by potentiometer. |

---

## Without I2C LCD Adapter

## Test Code

```c
// include the library code:
#include <LiquidCrystal.h>

// Creates an LCD object. Parameters: (rs, enable, d4, d5, d6, d7)
LiquidCrystal lcd(12, 11, 5, 4, 3, 2);

void setup() 
{
	// set up the LCD's number of columns and rows:
	lcd.begin(16, 2);

	// Clears the LCD screen
	lcd.clear();
}

void loop() 
{
	// Print a message to the LCD.
	lcd.print(" Hello world!");

	// set the cursor to column 0, line 1
	// (note: line 1 is the second row, since counting begins with 0):
	lcd.setCursor(0, 1);
	// Print a message to the LCD.
	lcd.print(" LCD Tutorial");
}
```
## References
- Data Sheet
  - [https://www.vishay.com/docs/37314/lcd020n004l.pdf](https://www.vishay.com/docs/37314/lcd020n004l.pdf)
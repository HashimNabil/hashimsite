# 14. Networking and communications


In this week group assignment, we will be sending message between two projects, I will be working with Abdallah AlSafadi his board will be the Master and my board will be the Secondary board.

It is communication between two Atmega 328 boards connected by these pin (SDA, SCL, GND, VCC)


## **Master board (Amal Ashoor)**

I created another master and slave codes for ATmega328 board and ATtiny44 board, resoectively, using "Wire.h" and "TinyWire.h" in Arduino IDE. After uploading the following codes to the boards, I connected their GND, VCC, SDA, and SCL using wires. The master code is:


```
#include <Wire.h>                   // Wire library. 

void setup() { 
   Wire.begin();                  // To initialize the Wire library and join the I2C bus. 
}

void loop() {
  Wire.beginTransmission(1);      // To begin a transmission to the first I2C device.
  Wire.write("Y");                // To send the message.
  delay(100);
  Wire.write("Z");                // To send the message.
  delay(100);
  Wire.endTransmission(1);        // To ends a transmission to a the device.
  delay(1000);
  Wire.beginTransmission(2);       // To begin a transmission to the second I2C device.
  Wire.write("X");                 // To send the message.
  delay(100);
  Wire.write("M");                 // To send the message.
  delay(100);
  Wire.endTransmission(2);         // To ends a transmission to a the device.

}
```

While the slave code is:

```
#include <TinyWire.h>                 // Tiny Wire library for ATtiny microcontrollers 
#include <twi.h>  

int LED = 8 ;                         // The microcontroller Pin connect to the LED.

void setup() { 
  TinyWire.begin(2);                  // Join I2C with device address 2 
  TinyWire.onReceive(ledevent);       // To register a function to be called when a device receives a transmission
  pinMode(LED, OUTPUT);               // LED is an output.  
}


void loop() {
   delay (100);
}


void ledevent(){ 
  while(TinyWire.available()){              // To ensure that the connection is availabe
     if (TinyWire.read() == 'M'){          
         digitalWrite(LED,HIGH);            // Turn on the LED
         delay (1000); 
         digitalWrite(LED,LOW);             // Turn off the LED
     }  
  }
}
```

This  [video](https://fabacademy.org/2022/labs/uae/students/amal-ashoor/work18.html) shows the successful communication between the boards.



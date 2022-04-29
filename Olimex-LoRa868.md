For testing I ordered the LoRa868 module from OLIMEX. I had originally intended it for development with my Arduino boards. 
The first hurdles were the wiring as the documentation was difficult to read. 
But for this I have now written together a good documentation. 
The bigger problem is the power supply on the digital pins, which is only allowed to be 3.3V for this module, 
but a standard Arduino supplies 5V, which led to unexpected interference in the communication.

    You cannot connect direct with an Arduino Uno!
    You need a 3.3V Board (Arduino Nano 33 BLE, Arduino Due, Arduino Zero)

| Description   | Arduino Pin   | LORA868 Pin   | Color       |
| ------------- | ------------- | ------------- | ----------- |
| DIO0          | 2             | 11            | Grey        |
| Reset         | 9             | 10            | White       |
| SS (NSS)      | 10            | 6             | Yello       |
| MOSI          | 11            | 5             | Orange      |
| MISO          | 12            | 4             | Green       |
| SCK           | 13            | 3             | Blue        |

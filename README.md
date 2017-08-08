# Arduino galvanic skin response sketch

Using the [Blynk](http://www.blynk.cc) data visualisation app.

## Parts

* [ESP32 Thing](https://www.sparkfun.com/products/13907)
* [Grove GSR sensor](http://wiki.seeed.cc/Grove-GSR_Sensor/)

## Installation

1. Clone this repository.
2. Create a `secrets.h` file with these defines:
```Arduino
#define blynkAuthToken "token"
#define your_ssid "ssid"
#define your_password "password"
```
3. Connect the GSR sensor to your ESP32:

**ESP32** | **GSR**
--- | ---
GND | GND
3.3v | VCC
32 (analog) | SIG

4. Upload the code to an Arduino.
5. Watch the serial output to check it’s connected to the internet.
6. Open the Blank iOS/Android app, and connect a graph to `pin V5`.
# Soil Moisture Monitoring using NodeMCU ESP8266, Soil Moisture Sensor, 0.96 OLED Display and Buzzer

# Table of Contents
1. [Arduino Libraries](#arduino-libraries)
1. [Libraries Installation Steps](#libraries-installation-steps:)
1. [Connection](#connection)
1. [Pictures](#pictures)
## Pictures:
### 1) Architecture Diagram<br>
![Architecture Diagram](https://user-images.githubusercontent.com/59210571/165559785-e16c6ba9-9a4f-4e6c-8cf3-77a3e6e5f8a8.png) <br><br>
### 2) Connection Picture<br>
![Connection Picture](https://user-images.githubusercontent.com/59210571/165560382-26f7b4d6-885c-4fab-91ba-6fd7f8c3c8ce.jpeg) <br><br>
### 3) Website Screenshot<br>
![Screenshot 2022-04-24 192541](https://user-images.githubusercontent.com/59210571/165560924-317ee24a-dd6a-4ab2-9762-5d9252f9a51b.jpg) <br><br>

## Arduino Libraries:
```
1) SSD1306 by Adafruit version 1.2.9
2) GFX by Adafruit version 1.4.13
3) ESPAsyncWebServer 
4) ESPAsyncTCP
5) Dallasremperature by Miles Burton version 3.8.0
6) OneWire by Paul Stoffregen version 2.3.5
7) Blynk by Volodymyr Shymanskyy version 0.6.1
```
## Libraries Installation Steps:
```
You can install the following libraries by:
1) Open Arduino IDE
2) Go to Sketch
3) Click on Include library
4) Select Manage libraries
5) The library manager will open, you can search and install the following libraries.
```
### OR
```
You can install through the library.zip by:
1) Unzip the library.zip
2) Move the folder to default location "C:\Users\<username>\Documents\Arduino\"
3) There will be a library folder
4) Copy there
5) If you have used custom folder for your project then copy the library folder there
```
## Connection:
### 1) NodeMCU ESP8266 -> Soil Moisture
```
3V -> VCC
A0 -> AOUT
G -> GND
```
### 2) NodeMCU ESP8266 -> OLED
```
G -> GND
3V -> VCC
D1 -> SCL
D2 -> VDA
```
### 3) NodeMCU ESP8266 -> Buzzer
```
D5 -> +ve
G -> -ve 
```
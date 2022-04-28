# Soil Moisture Monitoring using NodeMCU ESP8266, Soil Moisture Sensor, 0.96 OLED Display, and Buzzer

# Table of Contents
1. [Hardware Requirements](#hardware-requirements)
2. [Arduino Libraries](#arduino-libraries)
3. [Libraries Installation Steps](#libraries-installation-steps)
4. [Connections](#connections)
5. [Procedure](#procedure)
6. [Convert Image to Adafruit GFX Bitmap Code](#adafruit-gfx-bitmap-code)
7. [Images](#images)
## Images:
### 1) Architecture Diagram<br>
![Architecture Diagram](https://user-images.githubusercontent.com/59210571/165559785-e16c6ba9-9a4f-4e6c-8cf3-77a3e6e5f8a8.png) <br><br>
### 2) Connection Picture<br>
![Connection Picture](https://user-images.githubusercontent.com/59210571/165560382-26f7b4d6-885c-4fab-91ba-6fd7f8c3c8ce.jpeg) <br><br>
### 3) Website<br>
![Screenshot 2022-04-24 192541](https://user-images.githubusercontent.com/59210571/165560924-317ee24a-dd6a-4ab2-9762-5d9252f9a51b.jpg) <br><br>

## Hardware Requirements:
```
1) NodeMCU ESP8266
2) Soil Moisture Sensor
3) 0.96 OLED Display
4) Buzzer
5) BreadBoard
6) Jumper Wires
7) USB Cable
```
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
You can install it from library.zip by:
1) Unzip the `libraries.zip`
2) Copy the folder to default location "C:\Users\<username>\Documents\Arduino\"
3) Paste there
4) If you have used a custom folder for your project then copy the library folder there
```
## Connections:
#### 1) NodeMCU ESP8266 -> Soil Moisture
```
3V -> VCC
A0 -> AOUT
G -> GND
```
#### 2) NodeMCU ESP8266 -> OLED
```
G -> GND
3V -> VCC
D1 -> SCL
D2 -> VDA
```
#### 3) NodeMCU ESP8266 -> Buzzer
```
D5 -> +ve
G -> -ve 
```
## Procedure:
### Steps:
1) Connect all the IoT devices according to the pin connection mentioned above.
2) then install all the Arduino libraries from the `library.zip` folder as mentioned above.
3) Copy the code to Arduino IDE.
4) Connect the NodeMCU ESP8266 with the laptop.
5) Then click on `Tools` from the Arduino IDE navbar and make sure the NodeMCU board is selected.
6) And also make sure that Port is selected ( It will be auto-selected on device connection ).
7) Code Steps:
```
1) In network credential, enter your wifi name and password.
2) If you want to change the OLED Display image, then follow the `Convert Image to Adafruit GFX Bitmap Code` steps.
```
8) After making the changes, click on `Verify` and then click on `Upload`
9) When the code gets uploaded successfully it will show this message `Hard resetting via RTS pin`.
10) Then click on `Serial Monitor` to get the website IP.
11) Copy the IP and paste it into your browser.
12) Hence, your IoT application is ready to monitor the soil moisture.
## Convert Image to Adafruit GFX Bitmap Code:
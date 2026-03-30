# Sensor-Station
Sensor Station with LCD
This project implements a multi-sensor station using an Arduino Uno. It reads data from a PIR motion sensor, an HC-SR04 ultrasonic distance sensor, and an MQ-2 gas sensor, and displays the results on a 16x2 I2C LCD.

Components Needed
Arduino Uno (or compatible board)
16x2 LCD with I2C Backpack
PIR Motion Sensor (e.g., HC-SR501)
Ultrasonic Distance Sensor (HC-SR04)
Gas Sensor (e.g., MQ-2)
Jumper wires and a breadboard
Wiring Guide
Component	Pin / Connection	Arduino Uno Pin
I2C LCD	SDA	A4
SCL	A5
VCC	5V
GND	GND
PIR Sensor	OUT / Signal	D2
VCC	5V
GND	GND
HC-SR04	TRIG	D3
ECHO	D4
VCC	5V
GND	GND
MQ Gas Sensor	A0 (Analog Out)	A0
VCC	5V
GND	GND
Note: Depending on your specific modules, some sensors might require calibration (like the MQ-2 gas sensor pot) or sensitivity adjustments (like the PIR sensor).

Libraries Used
LiquidCrystal_I2C by Frank de Brabander (v1.1.4)
Wire (built-in)
Usage
Wire the components according to the table above.
Build and Flash the code to your Arduino.
The LCD will display the distance (in cm), motion status (YES/NO), and the raw analog gas level (0-1023).
You can also open the Serial Monitor at 115200 baud to see the sensor logs.

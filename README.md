
## IoT-Based Temperature & Humidity Monitoring System
This project is an IoT-based Temperature and Humidity Monitoring System using an ESP32 microcontroller, DHT22 sensor, and ThingSpeak API for cloud data visualization. 
Link for the Thinkspeak: https://wokwi.com/projects/412436855704093697

# Features
1.Real-time Temperature and Humidity Monitoring
2.Data Logging on ThingSpeak Cloud
3.LED Alert System for Extreme Conditions
4.WiFi Connectivity for Remote Monitoring

# Tech Stack
1.Hardware: ESP32, DHT22 Sensor, LED
2.Software: Arduino IDE
3.Cloud: ThingSpeak API
4.Communication: WiFi

# Installation and Setup
1.Clone the repository
git clone https://github.com/yourusername/IoT-Temp-Humidity-Monitor.git
cd IoT-Temp-Humidity-Monitor
2.Install Arduino Libraries
i.DHT sensor library
ii.ESP32 WiFi library
iii.ThingSpeak library
3.Update WiFi and ThingSpeak Credentials
Modify the following lines in the code with your WiFi and ThingSpeak details
const char* WIFI_NAME = "Your_WiFi_Name";
const char* WIFI_PASSWORD = "Your_WiFi_Password";
const int myChannelNumber = Your_ThingSpeak_Channel_ID;
const char* myApiKey = "Your_ThingSpeak_API_Key";
4.Upload Code to ESP32
i.Connect ESP32 to your PC
ii.Select ESP32 Dev Module in Arduino IDE
iii.Upload the code

# How It Works
1.ESP32 connects to WiFi for internet access
2.DHT22 sensor reads temperature and humidity data
3.Data is uploaded to ThingSpeak Cloud every 15 seconds
4.LED turns on if values exceed limits, such as temperature above 35 degrees Celsius or humidity above 70 percent
5.Monitor data on the ThingSpeak Dashboard in real-time

# Expected Output in Serial Monitor

WiFi connected!
Local IP: 192.168.1.100
Temp: 29.5°C
Humidity: 50.3%
Data pushed successfully
---
# Future Improvements
1.Add an LCD display for local monitoring
2.Implement an email alert system for extreme conditions
3.Extend cloud support to Firebase or Google Sheets

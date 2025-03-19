# Dustduino

#
https://benb0jangles.github.io/Dustduino/
#
ESP32-S3-Nano Environmental Monitoring System
Overview
This project uses an ESP32-S3-Nano to create an environmental monitoring system that measures temperature, humidity, and dust particle concentration. The data is displayed on a 128x32 OLED screen and also sent to ThingSpeak for remote monitoring and data visualization.
Features

Real-time temperature and humidity monitoring using DHT22 sensor
Air quality monitoring with GP2Y1010AU0F dust sensor
Local display on 128x32 I2C OLED screen
WiFi connectivity for remote data transmission
Cloud data logging via ThingSpeak API
Web-based visualization with custom GitHub Pages dashboard

Hardware Components

ESP32-S3-Nano (Waveshare ESP32-S3-Nano)
DHT22 temperature and humidity sensor
GP2Y1010AU0F dust/particle sensor
128x32 I2C OLED display (SSD1306)
Connecting wires and breadboard

Software Dependencies

Adafruit GFX Library
Adafruit SSD1306 Library
DHT Sensor Library
ESP32 Arduino Core
WiFi and HTTPClient libraries

Installation

Connect hardware components (esp32-S3-nano board is pin-identical drop in replacement for Old Arduino Nano board)
Install required libraries in Arduino IDE
Update WiFi credentials and ThingSpeak API key in the code
Upload the sketch to the ESP32-S3-Nano
Verify serial output and OLED display

ThingSpeak Integration
The system sends data to ThingSpeak every 30 seconds:

Field 1: Temperature (°C)
Field 2: Humidity (%)
Field 3: Dust Density (mg/m³)

Web Dashboard
A live dashboard is available at https://benb0jangles.github.io/Dustduino/
Future Improvements

Add additional environmental sensors (CO2, VOC, etc.)
Implement local data logging to SD card
Add configurable alert thresholds for poor air quality
Create a custom PCB for more compact installation
Implement deep sleep for battery operation

License
This project is licensed under the MIT License - see the LICENSE file for details.
Acknowledgments

Adafruit for their excellent libraries
ThingSpeak for providing the IoT analytics platform
The ESP32 community for documentation and support

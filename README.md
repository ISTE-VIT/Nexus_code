# Smart Home Bot

A smart vacuum cleaner bot powered by NodeMCU ESP32 that features obstacle detection, environmental monitoring, and remote/manual control through the Blynk Cloud Platform. This project demonstrates the application of IoT and embedded systems to develop a semi-autonomous cleaning system.

## Features

- Vacuum Cleaning System – Basic automated cleaning mechanism.
- Obstacle Detection System – Prevents collisions using ultrasonic sensors.
- Environmental Monitoring – Live updates from environmental sensors (e.g., temperature, humidity, gas).
- Web Dashboard – Displays real-time sensor data using a lightweight web server.
- Manual Control – Bot movement controlled remotely via the Blynk Cloud Platform.
- Motor Driver Integration – Controlled bot motion using L298N motor driver.

![WhatsApp Image 2025-04-13 at 15 41 46_80c0c54e](https://github.com/user-attachments/assets/9bafef77-5a18-4e61-9f70-bb8dda8a1ce2)

## Tech Stack

- Microcontroller: NodeMCU ESP32
- Languages: C++, HTML, CSS
- Libraries/Frameworks: Blynk, ESP32WebServer, Adafruit Sensor Libraries
- Sensors:
  - DHT11 for temperature & humidity
  - MQ series gas sensors
  - Infrared Sensors for obstacle detection
- Motor Driver: L298N
- DC Motors

## Web Dashboard

A custom-built web server hosted on the ESP32 shows environmental data like:

- Temperature
- Humidity
- Gas Levels
- Flame Detection

> Accessed through the ESP32's local IP address.

![WhatsApp Image 2025-04-13 at 16 53 26_e04689ab](https://github.com/user-attachments/assets/79c27aba-9256-4262-9916-a337419292d2)


## Blynk Integration

The bot can be manually controlled through the Blynk mobile app using virtual buttons and sliders:

- Forward, backward, left, right motion
- On/Off toggle for vacuum function

## Setup Instructions

1. **Hardware Setup**:

   - Connect ESP32 to motors via L298N.
   - Connect sensors (DHT11, gas, ultrasonic) to GPIO pins.
   - Power up the vacuum motor and ensure a stable 5V supply.

2. **Software Setup**:

   - Install the required libraries in Arduino IDE.
   - Flash the ESP32 with the provided code.
   - Configure WiFi credentials and Blynk authentication token in the code.

3. **Access the Web Dashboard**:

   - Once connected to WiFi, check the Serial Monitor for the ESP32’s IP address.
   - Open the IP in any browser to view real-time data

   ***

## Made with ❤ by ISTE VIT

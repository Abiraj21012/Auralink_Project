# AuraLink – Smart Agentic IoT Device with LLM Backend

An intelligent IoT-powered personal assistant that combines ESP32, environmental sensors, MQTT communication, and Large Language Models (LLMs) to deliver real-time environmental monitoring, smart email notifications, and AI-generated motivational quotes.

## 📌 Project Overview

**AuraLink** is a smart IoT device designed to act as a personal digital companion. It collects real-time environmental data, processes information through an AI-powered backend, and delivers meaningful updates through an OLED display and RGB LED indicators.

The system integrates IoT hardware with AI capabilities to provide a smarter and more interactive workspace experience.

## ✨ Key Features

- **Environmental Monitoring:** Real-time temperature and humidity monitoring using ESP32-connected sensors.
- **AI-Powered Quote Generation:** Generates personalized motivational quotes using OpenAI models based on environmental conditions and time of day.
- **Smart Email Notifications:** Monitors Gmail email headers to identify urgent messages without accessing email body content.
- **Email Priority Classification:** Categorizes notifications into High, Normal, and Low priority levels.
- **MQTT Communication:** Enables lightweight, bidirectional communication between the ESP32 device and backend server.
- **Intelligent Display:** Displays environmental readings, motivational quotes, and email notifications through an OLED screen.
- **RGB LED Indicators:** Provides visual notifications for urgent emails, connectivity, and system status.
- **Motion Detection:** Uses a PIR sensor to detect human presence and optimize device activity.
- **Automatic Brightness Adjustment:** Uses an LDR sensor to adjust OLED brightness according to ambient lighting.
- **System Logging:** Maintains application logs, sensor readings, and service performance information.

## 🏗️ System Architecture

AuraLink follows a three-layer architecture:

### 1. Device Layer – ESP32
The physical IoT device responsible for collecting environmental data and displaying information.

- ESP32 microcontroller
- DHT22 / BME280 temperature and humidity sensor
- OLED / TFT display
- RGB LED
- PIR motion sensor
- LDR light sensor

### 2. Communication Layer – MQTT

MQTT provides lightweight communication between the ESP32 and backend server using a publish/subscribe architecture.

- ESP32 publishes environmental sensor readings.
- Backend subscribes to incoming sensor data.
- Backend publishes AI-generated responses and notifications.
- ESP32 receives and displays the processed information.

### 3. Cloud & Intelligence Layer – Backend

The backend processes incoming information and coordinates AI-powered services.

- Python-based backend
- MQTT message handling
- OpenAI API integration
- Email monitoring service
- AI quote generation service
- Logging and monitoring service
- MongoDB data storage

## 🧠 AI Integration

AuraLink integrates Large Language Models (LLMs) to provide intelligent and context-aware functionality.

**Quote Generation Agent**
- Uses OpenAI GPT models to generate motivational quotes.
- Considers temperature, humidity, and time of day.
- Generates short quotes optimized for OLED displays.
- Supports predefined fallback quotes when AI services are unavailable.

**Email Monitoring Service**
- Connects to Gmail through IMAP.
- Monitors email headers rather than reading email body content.
- Identifies urgent messages using keywords and sender patterns.
- Classifies emails according to priority.
- Uses caching to optimize email monitoring.

## 🔧 Technologies & Tools

| Category | Technologies |
|---|---|
| Microcontroller | ESP32 |
| Programming | Python, Arduino |
| Firmware Development | Arduino IDE |
| Communication Protocol | MQTT |
| AI Integration | OpenAI API, LLM |
| Backend | Python, Flask / Django architecture |
| Database | MongoDB |
| Email Integration | Gmail IMAP |
| Display | OLED / TFT |
| Sensors | DHT22 / BME280, PIR, LDR |
| Hardware Indicators | RGB LED |

## 🔌 Hardware Components

- ESP32 Microcontroller
- DHT22 / BME280 Sensor
- OLED / TFT Display
- RGB LED
- PIR Motion Sensor
- LDR Light Sensor
- Breadboard
- Jumper Wires

## 📊 Project Objectives

1. Develop an intelligent IoT device using ESP32.
2. Implement real-time temperature and humidity monitoring.
3. Establish reliable device-to-backend communication using MQTT.
4. Integrate LLM-powered services for personalized information.
5. Implement smart email monitoring and priority notifications.
6. Display AI-generated information through an OLED interface.
7. Improve user experience through intelligent lighting and motion detection.

## 👨‍💻 Project Information

**Project Name:** AuraLink – Smart Agentic IoT Device with LLM Backend

**Module:** IT4030 – Internet of Things

**Institution:** Sri Lanka Institute of Information Technology (SLIIT)

**Academic Group:** Group 56

### Contributors

- Wanigasinghe C.P.
- Dissanayake H. P. M. S. S.
- Kailashawarn R.A.K.K.

## 🎯 Conclusion

AuraLink demonstrates how Internet of Things technology and Artificial Intelligence can work together to create a smarter and more interactive environment.

By combining environmental sensing, MQTT communication, AI-powered services, and intelligent notifications, AuraLink provides a practical example of integrating embedded systems with modern AI technologies.

---

**Developed as an academic IoT project at SLIIT.**

<img width="1376" height="752" alt="IoT (AuraLink) Architecture Diagram (no watermark)" src="https://github.com/user-attachments/assets/55da5531-cfa7-4bf8-827f-fd284dc65343" />




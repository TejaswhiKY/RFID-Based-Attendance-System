📡 RFID-Based-Attendance-System

An Arduino-based smart attendance system that uses RFID technology to automate student attendance recording. 
The system verifies RFID cards, displays attendance status on an I2C LCD, shows real-time date & time using DS1307 RTC, and provides audio feedback through a buzzer.

📌 Project Overview

This project eliminates manual attendance marking by using RFID cards. Each student is assigned a unique RFID card. When scanned, the system:

Reads the card UID

Verifies authorization

Displays attendance result

Records time using RTC

Produces audio feedback

🚀 Features

📡 RFID authentication using RC522

📟 16x2 I2C LCD display

🕒 Real-time timestamp using DS1307 RTC

🔔 Buzzer alert system

✅ One long beep → Attendance Successful

❌ Two long beeps → Access Denied



🔌 Circuit Connections
🔹 RC522 → Arduino UNO (SPI)
| RC522 | Arduino |
| ----- | ------- |
| SDA   | D10     |
| SCK   | D13     |
| MOSI  | D11     |
| MISO  | D12     |
| RST   | D9      |
| 3.3V  | 3.3V    |
| GND   | GND     |
⚠ Important: RC522 must use 3.3V, not 5V.

🔹 I2C LCD → Arduino

| LCD | Arduino |
| --- | ------- |
| VCC | 5V      |
| GND | GND     |
| SDA | A4      |
| SCL | A5      |

🔹 DS1307 RTC → Arduino

| RTC | Arduino |
| --- | ------- |
| VCC | 5V      |
| GND | GND     |
| SDA | A4      |
| SCL | A5      |

🔹 Buzzer → Arduino

|     Buzzer      |  Arduino  |
| ----------------|-----------|
| Red wire +      |   D8      |
| Black wire -    |   GND     |





🖥 UID display via Serial Monitor

🔄 Expandable for multiple users

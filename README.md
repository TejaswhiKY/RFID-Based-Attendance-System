---------------------------------------------------------------------------------------------
📡 RFID-Based-Attendance-System
---------------------------------------------------------------------------------------------
An Arduino-based smart attendance system that uses RFID technology to automate student attendance recording. 
The system verifies RFID cards, displays attendance status on an I2C LCD, shows real-time date & time using DS1307 RTC, and provides audio feedback through a buzzer.

---------------------------------------------------------------------------------------------
📌 Project Overview
---------------------------------------------------------------------------------------------
This project eliminates manual attendance marking by using RFID cards. Each student is assigned a unique RFID card. When scanned, the system:

▪ Reads the card UID

▪ Verifies authorization

▪ Displays attendance result

▪ Records time using RTC

▪ Produces audio feedback

---------------------------------------------------------------------------------------------
🎯 Features
---------------------------------------------------------------------------------------------
📡 RFID Card Authentication

📟 16x2 LCD Display

🕒 Real-Time Attendance Timestamp

🔔 Audio Feedback System

                ✅ One long beep → Attendance Successful

                ❌ Two long beeps → Access Denied

🖥 Serial Monitor UID Display

🔄 Expandable for Multiple Students

---------------------------------------------------------------------------------------------

🔌 Circuit Connections
---------------------------------------------------------------------------------------------
🔹 RC522 RFID → Arduino UNO (SPI)
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
---------------------------------------------------------------------------------------------
🚀 Future Improvements
---------------------------------------------------------------------------------------------
• Multiple student database

• EEPROM attendance storage

• SD card data logging

• WiFi-based cloud attendance system

• Web dashboard integration

• Biometric + RFID hybrid system

---------------------------------------------------------------------------------------------
🧪 Simulation Platform
---------------------------------------------------------------------------------------------
✅ Wokwi Simulator

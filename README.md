Smart Safety Wearables System
Women Safety Band & Child Safety Locket
📌 Project Overview

This project is an IoT-based safety wearable system designed for two different use cases:

Women Safety Smart Band – for personal safety and emergency alerts

Child Safety Smart Locket – for child monitoring and protection

Both devices are connected to a Firebase-backed web application that allows guardians or family members to track location and receive emergency alerts in real time.

🧩 System Architecture

Wearable Device (Band / Locket)

GPS Module

Microcontroller (ESP32 / ESP8266)

Firebase Realtime Database

Web Application (Parent/Guardian Dashboard)

⌚ Women Safety Smart Band
🎯 Purpose

To provide women with a quick and reliable emergency alert system that can be triggered during unsafe situations.

🔑 Features – Women Safety Band

Real-time GPS location tracking

Dedicated SOS emergency button

Instant alert trigger when SOS is pressed

Live location updates stored in Firebase

Wearable wrist-band design for easy access

Does not require a mobile phone during emergency

🛠️ Hardware Used

ESP32 / ESP8266

GPS Module

Push Button (SOS)

Battery Power Supply

⚙️ Working Flow – Women Safety Band

User wears the smart band

GPS continuously tracks location

In an emergency, SOS button is pressed

Location and SOS status are sent to Firebase

Guardian/Family can view live location on web app

📿 Child Safety Smart Locket
🎯 Purpose

To help parents monitor and protect children, especially in public places, schools, or outdoor environments.

🔑 Features – Child Safety Locket

Real-time child location tracking

SOS button for emergency situations

Sends live GPS data to Firebase

Neck-worn locket design (less likely to be removed)

Can work independently from the smart band

Acts as a backup safety device

🛠️ Hardware Used (Still under process)

ESP32 / ESP8266

GPS Module

Push Button

Battery Module

⚙️ Working Flow – Child Safety Locket

Child wears the smart locket

GPS tracks location continuously

SOS button sends emergency signal

Location data is updated in Firebase

Parent monitors status via web application

🌐 Web Application (Common for Both)
🔑 Features

Secure login using Firebase Authentication

Displays live GPS location

Shows SOS alert status clearly

Real-time updates without page refresh

Simple UI for quick understanding

🔥 Firebase Services Used

Firebase Authentication – Secure login

Firebase Realtime Database – Live tracking and SOS alerts

Sample Database Structure
{
  "devices": {
    "women_band_01": {
      "latitude": 12.9716,
      "longitude": 77.5946,
      "sos": true
    },
    "child_locket_01": {
      "latitude": 12.9720,
      "longitude": 77.5951,
      "sos": false
    }
  }
}

🚀 Setup Instructions
Hardware Setup

Connect GPS module to ESP32

Connect SOS button

Upload device firmware

Power device using battery


🔮 Future Enhancements

Mobile app (Android/iOS)

Geo-fencing alerts

SMS/call alert integration

Smaller and waterproof hardware

Battery optimization

👥 Team Information

Team Size: 4

Project Type: IoT + Web Application

Category: Women Safety & Child Safety

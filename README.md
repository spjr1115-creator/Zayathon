🛡️ Smart Safety Wearables System
Women Safety Band & Child Safety Locket
📌 Project Overview

The Smart Safety Wearables System is an IoT-based safety solution designed to address two critical real-world safety concerns:

Women Safety during emergencies

Child Safety through real-time monitoring

The system consists of two wearable devices:

Women Safety Smart Band

Child Safety Smart Locket

Both devices are connected to a Firebase-backed web application, enabling guardians or family members to track live location and receive SOS alerts in real time.

🎯 Objectives

Provide instant emergency alert capability

Enable real-time location tracking

Create a simple and reliable safety monitoring system

Reduce dependency on mobile phones during emergencies

🧩 System Architecture

The system follows a device → cloud → web dashboard architecture.

Components:

Wearable Device (Band / Locket)

GPS Module

Microcontroller (ESP32 / ESP8266)

Firebase Realtime Database

Web Application (Parent / Guardian Dashboard)

⌚ Women Safety Smart Band
🎯 Purpose

To provide women with a quick and reliable emergency alert system that can be triggered instantly during unsafe situations.

🔑 Features

Real-time GPS location tracking

Dedicated SOS emergency button

Instant alert generation when SOS is pressed

Live location updates stored in Firebase

Wrist-band design for quick access

Works independently without a mobile phone

🛠️ Hardware Used

ESP32 / ESP8266

GPS Module

Push Button (SOS)

Battery Power Supply

⚙️ Working Flow

User wears the smart band

GPS continuously tracks the location

SOS button is pressed during an emergency

Location and SOS alert are sent to Firebase

Guardian views live status on the web dashboard

📿 Child Safety Smart Locket
🎯 Purpose

To help parents monitor and protect children, especially in public places, schools, and outdoor environments.

🔑 Features

Real-time child location tracking

SOS button for emergency situations

Sends live GPS data to Firebase

Neck-worn locket (less likely to be removed)

Works independently from the smart band

Acts as a backup safety device

🛠️ Hardware Used (Under Development)

ESP32 / ESP8266

GPS Module

Push Button

Battery Module

⚙️ Working Flow

Child wears the smart locket

GPS tracks location continuously

SOS button sends an emergency signal

Location data updates in Firebase

Parent monitors status via the web application

🌐 Web Application (Common for Both Devices)
🔑 Features

Secure login using Firebase Authentication

Displays live GPS location

Clearly shows SOS alert status

Real-time updates without page refresh

Simple and user-friendly interface

🔥 Firebase Services Used
🔐 Firebase Authentication

Secure login for parents and guardians

📡 Firebase Realtime Database

Stores live GPS location data

Stores SOS alert status

📁 Sample Database Structure
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
🔧 Hardware Setup

Connect GPS module to ESP32

Connect SOS push button

Upload firmware to the microcontroller

Power the device using a battery

⚠️ Limitations

GPS accuracy depends on signal availability

Battery life is limited

Hardware casing is prototype-level

No mobile application yet

🔮 Future Enhancements

Android / iOS mobile application

Geo-fencing alerts

SMS and call alert integration

Smaller and waterproof hardware design

Improved battery optimization

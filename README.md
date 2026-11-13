# 🤖 MediBot – AI-Powered Healthcare Telepresence Robot

An IoT-based healthcare telepresence robot prototype designed for remote mobility, assisted patient interaction, obstacle detection, and prototype health monitoring.

## 🚀 Overview

MediBot is a smart healthcare robotics prototype built using ESP32, Embedded C/C++, and Python. It combines robotic mobility, sensor-based obstacle detection, and remote communication to support assisted patient interaction.

The system uses a FastAPI backend and WebSockets for application operations, real-time movement commands, and device status communication.

## ✨ Key Features

- **Remote Mobility:** Remote robot movement using a mecanum-wheel drive system.
- **Obstacle Detection:** Ultrasonic sensors for detecting nearby obstacles.
- **Health Monitoring:** MAX30102 sensor for prototype heart-rate and SpO2 readings.
- **Real-Time Communication:** WebSockets for movement commands and device status updates.
- **Backend Integration:** FastAPI-based backend for application operations.
- **Data Management:** SQLite for storing application data.

## 🛠️ Tech Stack

**Hardware & Embedded Systems**
- ESP32
- Embedded C/C++
- Mecanum-Wheel Drive
- Ultrasonic Sensors
- MAX30102 Sensor

**Backend & Communication**
- Python
- FastAPI
- REST APIs
- WebSockets

**Database**
- SQLite

## 🏗️ System Architecture

1. ESP32 controls the robot's hardware and movement.
2. Mecanum wheels provide multi-directional movement.
3. Ultrasonic sensors detect obstacles.
4. MAX30102 collects prototype heart-rate and SpO2 readings.
5. FastAPI handles backend application operations.
6. WebSockets enable real-time movement commands and device status communication.
7. SQLite supports application data storage.

## 📁 Project Structure

```text
MediBot/
│
├── firmware/
│   ├── src/
│   └── include/
│
├── backend/
│   ├── app/
│   │   ├── routes/
│   │   ├── services/
│   │   ├── models/
│   │   └── main.py
│   │
│   └── requirements.txt
│
├── hardware/
│   └── circuit-diagrams/
│
├── docs/
│   └── images/
│
├── .gitignore
└── README.md
```

## ⚙️ Installation & Setup

### 1. Clone Repository

```bash
git clone YOUR_REPOSITORY_URL
cd MediBot
```

### 2. Setup Python Environment

```bash
cd backend
python3 -m venv venv
```

Activate the environment:

**Mac/Linux**
```bash
source venv/bin/activate
```

**Windows**
```bash
venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run Backend

```bash
uvicorn app.main:app --reload
```

### 5. Access API Documentation

```text
http://127.0.0.1:8000/docs
```

## 🎯 Project Objectives

- Explore IoT-based healthcare applications.
- Implement remote robotic mobility.
- Integrate embedded sensors with backend services.
- Understand real-time communication using WebSockets.
- Develop practical experience in robotics and embedded systems.

## 👨‍💻 Developer

**Samir Khan**

Computer Science & Engineering | Full Stack & IoT Developer

- Portfolio: https://samirk.site
- GitHub: https://github.com/samirkhan41
- LinkedIn: https://linkedin.com/in/samir-khan-649158358

---

⭐ If you find this project interesting, consider giving it a star!

**Disclaimer:** This is a prototype for educational and development purposes. Sensor readings are not intended for medical diagnosis or clinical decision-making.

# 🤖 FLEXIBOT

FLEXIBOT is a smart, remotely controlled robotic system powered by BBC micro:bit.
It supports real-time control, telemetry, and future AI-based navigation.

---

## 🚀 Features

* 🎮 Real-time motor control (forward, reverse, turning)
* 📡 Bluetooth communication (Micro:bit ↔ Android)
* 📊 Telemetry (distance + battery monitoring)
* 🧭 Expandable for compass navigation
* ☁️ Cloud-ready backend (Node.js)
* 📱 Android control app
* 📈 Live dashboard (web)

---

## 🏗️ System Architecture

Micro:bit → Bluetooth → Android App → Cloud API → Dashboard

---

## 🔧 Hardware Requirements

* BBC micro:bit
* Motor driver (L298N or similar)
* DC motors
* Ultrasonic sensor (HC-SR04)
* Battery pack

---

## ⚙️ Setup Instructions

### 1. Firmware (Micro:bit)

* Open MakeCode
* Paste code from `/firmware/microbit/flexibot.ts`
* Flash to device

### 2. Backend

```bash
cd backend
npm install
node server.js
```

### 3. Dashboard

Open:

```
dashboard/index.html
```

---

## 📡 API Endpoints

| Method | Endpoint   | Description      |
| ------ | ---------- | ---------------- |
| POST   | /command   | Send control cmd |
| GET    | /telemetry | Get robot data   |

---

## 📱 Android App

* Connects via Bluetooth
* Sends commands to robot
* Displays live telemetry

---

## 🧪 Future Improvements

* AI obstacle avoidance
* GPS tracking
* Autonomous mode

---

## 👤 Author

Joshua Ansah Adjei

---

## 📄 License

MIT License

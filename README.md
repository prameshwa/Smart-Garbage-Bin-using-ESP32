# 🤖 Smart Garbage Bin Robot (ESP32)

## 📌 Project Description

The **Smart Garbage Bin Robot** is an intelligent, multi-mode robotic system built using **ESP32**, designed to automate garbage collection movement with both **autonomous and manual control**.

This robot can be controlled through:

* 🌐 **Web Interface**
* 📱 **Mobile App (APK)**
* ☁️ **Firebase (Realtime Database)**

The system allows seamless switching between different movement modes using Firebase and the website, making it flexible, scalable, and user-friendly.

---

## 🚀 Features

* 🔄 **Multi-Control System**

  * Control via Website
  * Control via Mobile App (APK)
  * Control via Firebase (Cloud)

* 🔁 **Three Movement Modes**

  1. **Manual Mode** – User controls robot in real-time
  2. **Line Following Mode** – Robot follows a predefined path
  3. **Random Mode** – Robot moves autonomously with random decisions

* ☁️ **Firebase Integration**

  * Real-time command updates
  * Mode switching from anywhere
  * Synchronization between app and website

* 📡 **ESP32 Wi-Fi Connectivity**

  * Enables cloud communication
  * Fast and efficient data handling

---

## 🧠 System Architecture

```
Mobile App / Website
         │
         ▼
     Firebase
         │
         ▼
       ESP32
         │
         ▼
     Robot Motors
```

* Commands are sent from **Mobile App or Website**
* Stored and updated in **Firebase Realtime Database**
* ESP32 reads data and executes actions

---

## ⚙️ Modes Explanation

### 🕹️ Manual Mode

* User directly controls robot movement (forward, backward, left, right)
* Controlled via:

  * Mobile App
  * Website

---

### 🧭 Line Following Mode

* Robot uses sensors to detect and follow a line path
* Ideal for structured environments

---

### 🎲 Random Mode

* Robot moves autonomously
* Makes random navigation decisions
* Useful for exploration or automatic garbage collection

---

## 🌐 Control System

### 1. Website Control

* Switch between modes
* Send movement commands
* Real-time updates via Firebase

### 2. Mobile App (APK)

* User-friendly interface
* Manual control buttons

### 3. Firebase Control

* Central control system
* Stores:

  * Mode state
  * Movement commands
* Syncs all platforms

---

## 🛠️ Technologies Used

* **ESP32 (Microcontroller)**
* **Firebase Realtime Database**
* **Arduino IDE (C/C++)**
* **Web Technologies (HTML, CSS, JavaScript)**
* **Android APK (Mobile App)**

---

## 🔌 Hardware Components

* ESP32
* Motor Driver (L298N)
* DC Motors
* IR sensors
* Power Supply
* Chassis
* Ultrasonic sensor

---

## 📲 How It Works

1. User selects mode (Manual / Line / Random)
2. Mode is updated in Firebase
3. ESP32 reads the mode
4. Robot executes behavior:

   * Manual → waits for commands
   * Line → follows path
   * Random → moves autonomously

---

## 📁 Project Structure

```
/robot-code
   └── robot_code.ino

/web-app
   └── index.html

/mobile-app
   └── app.apk

/firebase
   └── configuration details
```

---

## ▶️ Getting Started

### 1. Setup ESP32

* Install Arduino IDE
* Add ESP32 board
* Upload `robot_code.ino`

### 2. Configure Firebase

* Create Firebase project
* Enable Realtime Database
* Add credentials to ESP32 code

### 3. Run Web App

* Open website
* Connect to Firebase

### 4. Install Mobile App

* Install APK on your phone
* Start controlling the robot

---

## 🔮 Future Improvements

* Obstacle avoidance (Ultrasonic sensor)
* Camera integration (Live streaming)
* AI-based path optimization
* Voice control

---

## 🤝 Contribution

this is a  four member group project for Iot and Robotics module

---


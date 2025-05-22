# 🏠 Centralized Hub Home Automation (CHHA)

> 🧑‍💻 Developed by **Amirul Qayyum Sikambar**  
> 🎓 Final Year Project @ Universiti Malaysia Sabah (FCI)  
> ✉️ amirul2278@gmail.com

---

## 📖 Abstract

In Malaysia, IoT adoption is accelerating — yet most solutions are expensive, vendor-locked, and fragmented. This project proposes a **cost-effective and centralized IoT system** using:

- 🖥️ **Raspberry Pi** as server  
- 📡 **ESP-based microcontrollers** as clients  
- 🔄 **MQTT protocol** for communication  
- 🌐 **Flask** for the web interface

This system aims to democratize IoT access for hobbyists, small tech stores, and ISPs, providing key functionalities like dashboarding, automation, scheduling, and device control — without subscription fees.

---

## 🎯 Objectives

1. 🛠️ **Design** IoT infrastructure using MQTT for communication  
2. 🔗 **Develop** centralized system using Raspberry Pi (server) and ESP (client)  
3. 🧪 **Evaluate** general functionality via usability & black box testing  

---

## 🧰 System Requirements

To run this project smoothly, make sure you have the following:

- 🐧 **Linux OS** – Any distro should work, but:
  - ✅ 64-bit is recommended  
  - 🧩 Ensure USB WiFi dongle is compatible with your Linux version  
- 🍓 **Raspberry Pi 3 or 4** – Ideal as the central server  
  - Other models *may* work with tweaks  
- 💻 **Old Laptop Option** – Got an old Celeron or ThinkPad lying around?  
  - Even a ~2007 machine can run this  
  - 🔌 Try to stay under **45W power draw** for efficiency  
- 📶 **ESP8266 or ESP32** – Any ESP board should be supported  
- 🌐 **Minimum 2 Network Interfaces**
  - Recommended: 1× Wi-Fi + 1× Ethernet for local LAN + MQTT handling  

---

## 🧩 Modules

### 1. 📊 Dashboard
- CRUD interface for live widgets & sensor data  
- Auto-updates states from MQTT payloads  

### 2. 🔌 Device Management
- Add/manage ESP-based devices via topics  
- Control actuators and read sensors  

### 3. ⏰ Timer & Scheduler
- Set custom timers & weekly schedules  
- Trigger device actions automatically  

### 4. 💾 Backup & Restore
- Save and restore `.db` file configurations  
- Ensures easy migration or reset  

### 5. 👥 User Management
- Create/manage accounts and roles  
- Role-based access control for added security  

### 6. 🗺️ Zone Management
- Organize devices by rooms/zones  
- Manage actions zone-wise  

### 7. 💬 Feedback
- Submit and review system feedback  
- Helps improve usability  

### 8. ⚙️ Automation Rules
- Define logic-based triggers (e.g., "if sensor A = X, turn ON relay B")  
- MQTT-based rule execution  

---

## ⚙️ Technology Stack

| Tech | Purpose |
|------|---------|
| 🐍 Flask | Web framework (Python) |
| 🔌 MQTT (Mosquitto) | Real-time communication |
| 💽 SQLAlchemy | ORM for database handling |
| 🌐 HTML/CSS | Web interface |
| 🧠 ESP8266/NodeMCU | IoT clients |
| 🖥️ Raspberry Pi | Local server |

---

## ⚠️ Limitations and weaknesses

- 🔒 No encryption or secure auth (yet)  
- 🕒 Latency in automation triggers (due to blocking code)  
- 🧱 Not cloud-compatible or scalable  
- 🧮 SQL-based DB limits flexibility (Firebase preferred)  
- 🧵 No threading for background tasks (resource constraints)  
- 📡 MQTT traffic not encrypted  

---

## 🔮 Future Work

While this project lays the groundwork for **CHHA (Centralized Hub Home Automation)**, several enhancements are being considered for its next-generation evolution, known as **GCHHA (Greater Centralized Hub Home Automation)** — a more scalable, secure, and modular IoT platform:

- 🐳 **Containerization with Docker**  
  Ensure consistent deployment and improved modularity for IoT services

- ⚙️ **Migration to Node.js**  
  Leverage non-blocking I/O for improved async performance and better real-time handling

- ☁️ **Cloud API Integrations**  
  Sync data with external platforms (e.g., analytics, weather, or cloud automation)

- 🔐 **Secure MQTT with TLS & Authentication**  
  Encrypt device communication and implement proper identity verification

- 🔥 **Firebase Real-Time DB**  
  Replace SQL-based backend with a scalable, real-time NoSQL database suited for large-scale IoT applications

---

## 📚 References (just to fullfil the acadamic purpuses)

- [1] S. Tiwari, “IoT Application in Malaysia” [DOI:10.3570/bjost.2022.4.1-11]  
- [2] Hunkeler et al., "MQTT-S Protocol"  
- [3] IEEE IoT-SIU, 2019 — Electrical Surveillance  
- [4] ACCAI 2022 — Smart Home via Python + RPi  
- [5] IEEE Voice-Controlled IoT System  
- [6] ACCESS 2021 — Smart Switch w/ Bluetooth  
- [7] IoT-SIU — Smart Kitchen Web App  

---

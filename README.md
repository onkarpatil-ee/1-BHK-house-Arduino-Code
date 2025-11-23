## 🏠 TechNest: 1 BHK Smart Home Automation System

This project implements a complete smart home automation system for a **1 BHK (one-bedroom-hall-kitchen)** dwelling, offering both automatic and manual control of electrical loads like lights and fans, enhanced with smart security features. The core of the system is built around the **ESP32** and **Arduino UNO** platforms, utilizing a **4-channel relay module** for load control.

---

### ✨ Key Features

**Dual Control Modes:** Supports both **Automatic and Manually Controllable** operation.
**Smart Control:** Appliances can be controlled via the **ESP32 Rain Maker mobile application**, **Voice** commands, **Google Gemini**, and **Google Home**.
**Security:** Features a **Smart RFID-Based Door locking system**.
**Motion Lighting:** Implements a **Smart motion based parking lighting setup** using **PIR sensors** for automatic light control.
**Scheduling:** Includes **Timer based ON/OFF** functionality for user convenience.

---

### 💻 Control Panel Visual Mockup (Static)

This section simulates the look of the control dashboard using a GitHub-compatible Markdown table with inline styling for the color status indicators.

| Control Card: Hall Appliances | Control Card: Parking/Washroom | Control Card: Smart Door Lock |
| :--- | :--- | :--- |
| **Living Hall Control** | **Parking/Washroom Light** | **Smart Door Lock** |
| *Status: Manual Mode* | *Mode: Automatic (PIR)* | *System: Active* |
| **Light 1 (Relay 1)**: <span style="background-color: #e74c3c; color: white; padding: 3px 6px; border-radius: 4px; font-weight: bold;">OFF</span> | **Parking Light**: <span style="background-color: #3498db; color: white; padding: 3px 6px; border-radius: 4px; font-weight: bold;">AUTO ON</span> | **Front Door**: <span style="background-color: #c0392b; color: white; padding: 3px 6px; border-radius: 4px; font-weight: bold;">LOCKED</span> |
| **Fan (Relay 2)**: <span style="background-color: #2ecc71; color: white; padding: 3px 6px; border-radius: 4px; font-weight: bold;">ON</span> | PIR Sensor: Motion Detected | LCD Status: Locked  |
| <button type="button" style="background-color: #3498db; color: white; border: none; padding: 5px 10px; border-radius: 4px; cursor: pointer;">Toggle Light</button> | | <button type="button" style="background-color: #3498db; color: white; border: none; padding: 5px 10px; border-radius: 4px; cursor: pointer;">Remote Unlock</button> |

---

### ⚙️ Wiring and Block Diagrams

#### 1. Main Home Automation Wiring (ESP32)
The main automation uses the ESP32 to connect to a 4-channel relay module, allowing remote or manual switching of up to four loads (like lights and fans).



#### 2. Smart Door System Wiring (Arduino UNO)

This security system is managed by the Arduino UNO and features the **RFID Module**, **LCD Display** (to show locked/unlocked status), and a **Servo Motor** for the locking mechanism.



#### 3. Automatic Parking Light Wiring (Arduino UNO)

This system uses an Arduino UNO to control a single channel relay connected to a bulb, triggered by a **PIR Sensor** to detect motion in areas like a parking space.



---

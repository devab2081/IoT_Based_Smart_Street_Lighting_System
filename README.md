# 💡 IoT Smart Street Lighting System  
### Hackathon Project – Smart Hack 2025 (TamilNadu)

This project demonstrates an **automatic smart street lighting system** using **Arduino UNO**, **LDR**, **PIR sensor**, and a **Relay module** to control AC street lights based on ambient light and human movement.

When it becomes dark → Light turns ON automatically  
When person is detected → Light becomes brighter  
No person detected → Light returns to dim/off state  

---

# 📌 Features

- 🌙 **Auto ON/OFF using LDR** (day/night detection)  
- 🚶‍♂️ **Motion-based activation using PIR sensor**  
- ⚡ **Relay-based AC lamp control**  
- 🔋 Saves electricity  
- 🛠 Simple + low-cost hardware  
- 🧠 Can be extended into full IoT system (ESP32, MQTT, Cloud)

---

# 🖼️ Updated Circuit Diagram

Below is the wiring diagram you uploaded.  
I have updated the README to correctly show it:

![Smart Street Light Circuit](circuit.jpg)

---

# 🔌 **Circuit Explanation**

### 🔹 **LDR (Light Sensor)**
- Detects ambient light  
- Connected to **Analog pin A0**  
- Used to determine day or night  

### 🔹 **PIR Sensor (Motion Detector)**
- Output connected to **Digital pin 8**  
- Detects human movement  
- Activates lamp only when needed  

### 🔹 **Relay Module**
- Coil controlled by Arduino digital output (**pin 7**)  
- Switches AC bulb ON/OFF safely  
- AC **neutral** goes directly → AC **live** passes through relay  

### 🔹 **Arduino UNO**
- Reads LDR value  
- Reads PIR digital output  
- Drives relay based on conditions  

---

# 📂 Files Included (Updated)

```
Smart Street Lights - Source/
│── circuit.jpg              # Updated circuit diagram
│── README.md                # Documentation (this file)
│── *.ino or *.cpp           # Arduino source code (add your sketch here)
└── (Add any sensor libraries if required)
```

---

# 🔧 Arduino Logic (Working Principle)

```
IF (LDR detects DARK) THEN
    IF (PIR detects motion)
         Turn ON street light (relay HIGH)
    ELSE
         Dim or keep OFF (relay LOW)
ELSE
    Turn OFF street light (daytime)
```

---

# 🛠 Hardware Required

- Arduino UNO  
- LDR + 10k resistor  
- PIR Motion Sensor  
- Relay Module (5V)  
- Connecting wires  
- AC Bulb (Test lamp)  
- Breadboard  

---

# ⚠️ Safety Note (Important!)

- Relay switches **high voltage AC**  
- Make sure to insulate live wires properly  
- Keep AC wiring away from Arduino/low-voltage components  
- Only test under supervision  

---

# 🚀 Future Improvements (Recommended)

- Add ESP32 → make it fully IoT  
- Add MQTT + Cloud Dashboard  
- Measure energy usage  
- Add automatic fault detection (lamp failure)  
- Add solar panel with battery backup  

---

# 🏅 Credits

This project was designed and developed by:

### **Devadharsan B**  
IoT | Embedded Systems | Arduino | Smart Electronics Enthusiast  

Created as part of **Smart Street Lighting System** project work  
and demonstrated during **Smart Hack 2025 (TamilNadu)**.



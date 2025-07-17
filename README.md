# 🏥 Remote Patient Monitoring System

An IoT-based health monitoring system designed to track vital parameters such as ECG, body temperature, SpO₂ (oxygen level), heart rate, and motion (fall detection). It enables real-time communication between patients and healthcare providers using mobile application integration.

---

## 🧠 Abstract

This project addresses the challenges of continuous health monitoring, especially for patients in remote or underserved areas. The system uses multiple sensors (ECG, pulse, temperature, SpO₂, motion) connected to an ESP32 microcontroller. Data is sent to a mobile app via Wi-Fi. If abnormal readings are detected, alerts (including SMS notifications) are generated to notify doctors in real time. This enables proactive and timely medical response.

---

## 🌟 Features

- Monitors ECG, heart rate, oxygen saturation (SpO₂), temperature, and fall detection.
- Real-time wireless data transmission to mobile app.
- SMS alerts to healthcare providers in case of abnormal readings.
- Compact and portable hardware setup.
- Blynk-based mobile app integration.
- Low-cost and scalable for rural deployment.

---

## 🛠️ System Overview

**Control Unit:** ESP32 Microcontroller  
**Sensors:**
- MAX30102 – Heart Rate & SpO₂
- DS18B20 – Body Temperature
- AD8232 – ECG Signal
- MPU6050 – Motion/Fall Detection

<img width="697" height="356" alt="block diagram" src="https://github.com/user-attachments/assets/888e8bdc-7125-4b10-941c-af1bc8595e03" />


---

## 🔩 Hardware Components

| Component            | Quantity | Description                        |
|----------------------|----------|------------------------------------|
| ESP32 Dev Board      | 1        | Main microcontroller with Wi-Fi    |
| MAX30102 Sensor      | 1        | Measures heart rate and SpO₂       |
| DS18B20 Sensor       | 1        | Measures body temperature          |
| AD8232 Sensor        | 1        | Captures ECG signal                |
| MPU6050 Sensor       | 1        | Tracks motion / fall detection     |
| PCB + Case           | 1 each   | Prototyping base and housing       |
| Jumper Wires         | 100      | Hardware interfacing               |
| Mobile USB Cable     | 1        | Power supply and data              |


---

## 🔄 Methodology

1. Sensors continuously collect vital data.
2. ESP32 processes raw signals, applies filtering.
3. Data is wirelessly transmitted to Blynk mobile app.
4. SMS alerts are triggered if parameters exceed thresholds.
5. All processing occurs in near real-time.

📱 **Mobile Interface**:  
The Blynk app displays:
- Heart Rate (BPM)
- Oxygen Level (SpO₂ %)
- Body Temperature (°C)
- Fall Detection alert (if any)
- ECG waveform
<img width="997" height="568" alt="blynk app interface" src="https://github.com/user-attachments/assets/54e09f84-e896-4448-9c45-d06e48d836d3" />


---

## ✅ Results

- **Accuracy:** 80%+ for health readings.
- **Heart Rate Range:** 88–125 BPM  
- **SpO₂ Range:** 63–96%  
- **Temperature Range:** 28–37.2°C  
- **Latency:** ~3 sec for HR/SpO₂, ~62 ms for temperature  
- **Feedback:** Users found it portable, fast, and informative.

---

## 🚀 Applications

- Real-time remote patient health monitoring
- Fitness and wellness tracking
- Elderly care and fall detection
- Post-operative rehab support
- Pandemic symptom tracking (fever, O₂ drop)
- Telemedicine and home-based care

---

## 🔮 Future Scope

- Add blood pressure monitoring
- Improve battery efficiency and life
- Use ML for health anomaly prediction
- Implement encrypted cloud storage
- Add solar-based power options
- Validate with a larger patient base

---



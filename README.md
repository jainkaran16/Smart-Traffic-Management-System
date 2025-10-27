## 🧠 Overview
This project proposes a **Smart Adaptive Traffic Management System** that dynamically controls traffic signals based on **real-time vehicle density** and **emergency vehicle detection** using **YOLO (You Only Look Once)** and **Arduino-based automation**. It ensures faster movement for ambulances and optimized green light durations for heavy lanes, reducing congestion and improving urban safety—while remaining **low-cost and scalable**.

- Real-time vehicle detection and lane density estimation with **over 90% accuracy**, enabling dynamic signal adjustments to optimize flow.
- **Emergency vehicle prioritization** cut ambulance wait times by **~70%** and boosted green time for high-density lanes by **up to 3.5×**.
- **~25% reduction in overall congestion** via dynamic signal allocation, with live outputs driven on **Arduino LED arrays**.

---

## ✨ Features
- 🚗 **YOLO-based vehicle detection** for real-time density analysis  
- 🚑 **Emergency vehicle prioritization** using Boolean flags  
- ⏱️ **Adaptive green-time calculation** via a mathematical model  
- 🧩 **Arduino UNO automation** controlling 4-way LED signal simulation  
- 💡 **Low-cost, scalable system** without GPS/RFID dependency  

---

## ⚙️ Methodology

1. **Input:** Live camera feeds from four lanes  
2. **Detection:** YOLO identifies vehicles & ambulances  
3. **Computation:**  
   - Calculates lane density  
   - Applies the adaptive timing formula  
   - Prioritizes lanes with emergency vehicles  
4. **Control:** Arduino adjusts signal LEDs (Red, Yellow, Green) dynamically  

**Green Time Formula**

`GreenTime_i = G_i × (1 + D_i/A_i) × (1 + Amb) + 0.25 × Amb × T_amb`

---

## 🧪 Results

<img width="571" height="343" alt="Screenshot 2025-10-27 at 11 30 50 AM" src="https://github.com/user-attachments/assets/ecad24e7-8bb7-470b-a398-f26d8a9eb0df" />

<img width="581" height="352" alt="Screenshot 2025-10-27 at 11 32 10 AM" src="https://github.com/user-attachments/assets/902b11e6-fd98-4976-bbae-930f23fa9f5a" />

![WhatsApp Image 2025-10-27 at 11 37 11](https://github.com/user-attachments/assets/540133f0-e8d4-4f8a-9702-9847c58355d7)

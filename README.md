# 🧭 Arduino Ultrasonic Radar System

A radar system using **Arduino UNO**, **HC-SR04 Ultrasonic Sensor**, and **SG90 Servo Motor**, visualized in real-time using **Processing IDE**.

---

## 📸 Circuit Diagram
![Circuit Diagram](Circuit_Diagram.png)

---

## ⚙️ Components Used
- Arduino UNO  
- HC-SR04 Ultrasonic Sensor  
- SG90 Servo Motor  
- Jumper wires  
- Breadboard  
- USB Cable  
- Processing IDE (for visualization)

---

## 🧠 How It Works
1. Arduino rotates the servo from **15° to 165°** and measures distance using the ultrasonic sensor.  
2. Arduino sends serial data in the format:

angle,distance.

3. Processing IDE reads this data and visualizes it like a **radar sweep**:
- Green line → scanning beam  
- Red dots → detected objects (<40 cm)  
- “Out of Range” → objects beyond 40 cm  

---

## 💻 Folder Structure

Arduino-Ultrasonic-Radar/ ├── Arduino_Code/ │   └── ultrasonic_radar.ino ├── Processing_Code/ │   └── radar_visualization.pde ├── Circuit_Diagram.png └── README.md

---

## 🏃‍♂️ How to Run
1. Connect Arduino to PC.  
2. Upload `ultrasonic_radar.ino` using **Arduino IDE**.  
3. Open `radar_visualization.pde` in **Processing IDE**.  
4. Update COM port in Processing code if needed:
   ```java
   myPort = new Serial(this, "COM5", 9600);

5. Run Processing sketch → watch real-time radar visualization.



---

📌 Notes

Make sure Arduino and Processing IDE are installed.

Use the correct COM port in Processing IDE.

Works best on full-screen mode.


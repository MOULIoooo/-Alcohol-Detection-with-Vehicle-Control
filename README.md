# -Alcohol-Detection-with-Vehicle-Control
This project aims to enhance vehicle safety by integrating an alcohol detection module with braking control and police alert features. When alcohol is detected from the driver's breath, the system immediately disables the vehicle’s movement and sends the driver’s identity to a connected police database.
## 📌 Components Used

- Arduino Uno / ESP32
- MQ-3 Alcohol Sensor
- Servo Motor (for simulating brake lock)
- Buzzer
- LCD Display (optional)
- GSM Module / ESP32 for police notification
- Power Supply / Battery
- Jumper wires, breadboard

---

## ⚙️ Working Principle

1. The MQ-3 sensor detects alcohol vapor from the driver's breath.
2. If the alcohol level exceeds a preset threshold:
   - A buzzer is activated.
   - The servo motor simulates a brake lock.
   - A message (via GSM or Wi-Fi) is sent to a police control database.
3. If no alcohol is detected, the vehicle operates normally.

---

## 🔧 How to Run

1. Upload the Arduino/ESP32 code to your board.
2. Power the system and place the alcohol sensor near the driver’s seat.
3. Observe behavior based on sensor readings.

---

## 📸 Project Images

*(Upload real images to your GitHub and display them here)*

---

## 📹 Demo Video

[Watch the demo](https://your-demo-link)

---

## 🧠 Developed By

👨‍💻 Mouli S  
St. Joseph's College of Engineering  
Department of EEE

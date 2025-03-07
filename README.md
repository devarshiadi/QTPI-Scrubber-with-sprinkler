# 🧽 Scrubber with Sprinkler 🚿

## 🔹 Introduction
The **"Scrubber with Sprinkler"** is a smart cleaning system that integrates a motor-driven scrubber with a water-sprinkling mechanism. The system is controlled via a **mobile app 📱**, which connects to an **IoT device** over **Bluetooth 🔵**. The app allows users to **turn the sprinkler ON/OFF 💦** and monitor **sensor values in real-time 📊**.

## ⭐ Features
✅ **Bluetooth Connectivity**: Connects to an IoT device via Bluetooth.
✅ **Motor-Controlled Scrubber**: Runs a motor-driven cleaning brush based on sensor input.
✅ **Water Sprinkler**: Activates or deactivates a water pump for sprinkling.
✅ **IR Sensor Integration**: Detects obstacles or conditions and adjusts motor speed.
✅ **User-friendly Interface**: Simple UI with labels, checkboxes, and alerts.

---

## 🛠️ Components Used

### **🎨 Frontend (User Interface)**
- **📡 ListPicker (CONNECT Button)**: Allows users to select and connect a Bluetooth device.
- **🏷️ Labels**: Display information such as sensor values.
  - `IR_SENSOR_VALUE`: Shows the real-time IR sensor value.
- **☑️ Checkbox (Sprinkler ON/OFF)**: Enables or disables the water sprinkler.
- **🔔 Notifier**: Displays connection status and alerts to users.

### **⚙️ Backend (Logic & Control)**
- **🔵 Bluetooth Client**: Handles connection between the app and the IoT device.
- **🔄 Motor**: Rotates the scrubber based on sensor data.
- **💦 Pump Motor**: Controls the water sprinkler.
- **📡 IR Sensor**: Detects objects or surface conditions and adjusts motor speed.

---

## 🚀 Working Mechanism

### **📶 Bluetooth Connection**
1. The user taps the **CONNECT 🔘** button.
2. A list of available **Bluetooth devices** appears.
3. Upon selecting a device, the app attempts to **connect 🔄**.
4. ✅ If successful, it displays a **"CONNECTED ✅"** message.
5. ❌ If failed, it shows **"FAILED TO CONNECT ❌"**.

### **📡 IR Sensor & Motor Control**
1. The **IR sensor 👀** continuously monitors its environment.
2. The sensor value updates in the app (`IR_SENSOR_VALUE 📊`).
3. If the sensor detects an obstacle (or a specific condition), the scrubber motor rotates at **speed 200 ⚡**.
4. Otherwise, the scrubber motor stops (speed **0 🛑**).

### **💦 Sprinkler System**
1. The user toggles the **Sprinkler ON/OFF ☑️** checkbox.
2. If **checked**, the **pump motor runs at speed 200 🔄**, activating the sprinkler.
3. If **unchecked**, the **pump motor stops (speed 0 🛑)**.

---

## 🌍 Real-World Application: Automatic Floor Scrubber
Imagine a **robotic floor scrubber 🤖** in a **mall 🏢** or **hospital 🏥**:
- The **scrubber moves 🚗**, detects dirt (**IR sensor logic 📡**), and rotates its **cleaning brush 🧹**.
- The **sprinkler ensures water is sprayed 💦** when needed.
- The **Bluetooth-controlled app 📱** allows easy remote operation.

This simple yet effective system enhances **cleaning efficiency** and **automation**. 🏆

---

## 🎯 Summary
✅ The **app connects** to an IoT scrubber system via **Bluetooth**.
✅ The **IR sensor detects** conditions and **controls the scrubber motor**.
✅ The **user can toggle** the **water sprinkler** using a checkbox.
✅ The **app provides real-time updates and feedback**.

This project integrates **IoT 🤖, Bluetooth 🔵, and sensor-driven automation 📡** for a **smart cleaning solution**. 🏆

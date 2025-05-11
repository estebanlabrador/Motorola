# 🛠️ Compressed Air Engine: Project Motor.ola

**Team:** Motor.ola  
**Contributors:** Esteban Labrador de la Fuente, Inés Gadea, Manuel Candalija, Javier Barbero, Alberto Martínez, Antonio Treilhou  
**Course:** Ingenia MotorGEN – 1º MII 2023–2024  
**Tools Used:** Lathe, Milling Machine, Arduino, HX711, Proximity Sensors, SolidWorks

---

## ⚙️ Project Overview

The **Motor.ola** team developed and successfully fabricated a unique **compressed air engine** inspired by INNengine's opposed piston design. After three years of prior attempts, this iteration achieved operational success, combining innovative mechanical engineering, machining precision, and real-time electronic measurement.

---

## 🔩 Key Features

- **Opposed piston engine** based on a 4-cylinder 2-stroke configuration.
- Full mechanical manufacturing including:
  - Pistons, cylinders, valve body, camshaft, and support structure.
  - Custom valve system to control compressed air flow.
- Components fabricated via **machining (lathe, milling, drilling)** and **aluminum casting**.
- Structural improvements with customized rubber seals and tight tolerances to reduce air leaks.

---

## 🧪 Instrumentation & Sensors

### 🌀 RPM Measurement
- **Sensor:** Flying Fish IR proximity sensor
- **Method:** Detects reflective marks on the rotating cam
- **Output:** Live RPM reading using Arduino + OLED screen

### 🔧 Torque Measurement
- **Sensor:** Load cell connected to a **Prony brake**
- **Amplifier:** HX711 ADC
- **Arduino Program:** Converts load readings to torque and power

---

## 📊 Experimental Results

- **Max torque:** 1.3 Nm (vs 2.2 Nm design goal)  
- **Max RPM:** ~354 RPM (vs 600 RPM design)  
- **Power Curve:** Max output ~12 W, peaking near 100 RPM  
- **Key Limitation:** Air leakage and manual startup

![Sample Graph: Torque vs RPM](./images/torque_vs_rpm.png)

---

## 🔄 Suggested Improvements

- **Tighter valve machining** to reduce air leaks  
- **Consistent piston diameters** for better balance  
- **External starter system** (e.g., chainsaw pull-start adaptation)  
- **Fully automated data logging** for test cycles

---

## 🧰 Arduino & Code Highlights

- Integrated sensors with **Arduino Mega 2560**
- Output to both **OLED screen** and **serial monitor** for logging
- Measures:
  - Real-time torque (via load cell + HX711)
  - RPM (via IR proximity sensor)
- Implements filtering and debounce logic to ensure accurate readings

---

## 📂 Full Report

[📄 Download PDF Final Report](./Informe_Junio%20(1).pdf)

---

> _This project involved full-cycle engineering, from design to fabrication to instrumentation, showcasing hands-on mechanical and electronic systems integration. The success marks a milestone in compressed air engine prototyping within an academic setting._

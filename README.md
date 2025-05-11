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


# 🛠️ Compressed Air Engine – Project Motor.ola

**Team:** Motor.ola  
**Contributors:** Esteban Labrador de la Fuente, Inés Gadea, Manuel Candalija, Javier Barbero, Alberto Martínez, Antonio Treilhou  
**Course:** Ingenia MotorGEN – 1º MII 2023–2024  
**Tools & Platforms:** Lathe, Milling Machine, Casting, Arduino (HX711, IR Sensor), SolidWorks

---

## 🚀 Project Overview

This project aimed to design and fabricate a **non-conventional compressed air engine** inspired by the opposed piston layout of the INNengine. The resulting prototype features a **4-cylinder, 2-stroke air-powered engine** with minimal vibration and a compact footprint. After three years of failed attempts in previous iterations, the 2023–2024 team successfully delivered a fully operational engine.

---

## 🧠 Mechanical Design

- **Layout:** Opposed twin 2-stroke pistons (4 cylinders total), radially arranged
- **Valve System:** Central rotary valve with radial air distribution
- **Transmission:** Custom camshaft-driven expansion
- **Materials:** Aluminum for lightweight components; steel for structural and moving parts
- **CAD:** Designed in SolidWorks with detailed mechanical drawings for each part
- **Innovations:**
  - Air recovery and venting holes to reduce cross-cylinder pressurization
  - Custom intake/exhaust valve with dynamic sealing
  - Adjustable tension and alignment system using elastic inserts and 3D printed guides

---

## 🔧 Manufacturing Process

- **Machining:**
  - **Lathe:** Used for cylinders, pistons, connecting rods, cam, and valve housing. Each part was turned to tight tolerances (±0.1 mm).
  - **Milling:** Performed on the valve supports, mounting bases, and alignment flats.
  - **Drilling & Tapping:** Manual threading for pressure ports, bolt holes, and valve assembly.

- **Casting:**
  - Aluminum casting was used for complex components like the **cam** and **cylinder-valve base support**.
  - Wooden patterns and sand molds were used; post-casting cleanup included **facing, polishing**, and **manual finishing** with files and sandpaper.

- **Assembly Adjustments:**
  - Rubber gaskets were added between cylinders and cast supports to compensate for machining tolerance errors.
  - Coca-Cola can metal was recycled as shims to stabilize bearing retainers—a creative fix that improved performance.
  - A unique piston-cylinder pairing system was used: each piston was manually fitted to its cylinder to account for minor dimensional deviations.

---

## 🧪 Instrumentation and Electronics

### 🔩 Torque & RPM Measurement

- **Prony Brake:** A custom-designed friction brake using a leather belt and aluminum drum mounted to the output shaft.
- **Load Cell + HX711:** Measures tension in the brake assembly and calculates torque via known arm length.
- **Proximity Sensor:** Detects revolutions using a reflective marker on the cam.

### 📟 Arduino System

- **MCU:** Arduino Mega 2560
- **Display:** 0.96” OLED screen + serial monitor logging
- **Functionality:**
  - Converts sensor data to live torque and RPM readouts
  - Updates every 5 seconds for averaged values
  - Data exported via USB to CSV for analysis

---

## 📊 Performance Results

- **Max Torque:** 1.3 Nm  
- **Max RPM:** ~354 RPM  
- **Peak Power Output:** ~12 W at ~100 RPM  
- **Expected (Design):** 2.2 Nm and 600 RPM ⇒ 50 W  
- **Limiting Factors:** Air leakage and manual startup reduced max achievable performance.

---

## 🧩 Challenges and Fixes

| Challenge                                 | Solution                                                                 |
|------------------------------------------|--------------------------------------------------------------------------|
| Air leakage in valve system              | Added sealing vents + improved valve fit                                 |
| Casting dimensional inconsistencies      | Used gaskets and shims to ensure alignment                               |
| Oversized cylinder bore (1/4 cylinders)  | Fabricated custom piston with matching diameter                          |
| Sensor instability in bright lighting    | Tuned IR proximity sensor sensitivity for lab environment                |

---

## 🔄 Proposed Improvements

- Replace manual startup with an electric or recoil system (e.g., chainsaw starter)
- Improve valve-to-body tolerances for better sealing and efficiency
- Re-machine mis-sized cylinders for uniform piston-air demand balance
- Add automated data logging with SD card or wireless module

---

## 📄 Full Report

[📘 Download PDF Report](./Informe_Junio%20(1).pdf)

---

> _This project embodies the full engineering cycle: from CAD design to machining, casting, assembling, troubleshooting, instrumentation, and performance testing. It reflects a hands-on, creative approach to building a working pneumatic engine system from the ground up._

# RC Submarine HackClub Project

## Overview

This is a low-cost, advanced RC submarine designed for underwater robotics and STEM learning. The project is meant to be submitted for a HackClub grant and includes smart control, 3D printed body, and sensor integration.

---
<img width="600" height="333" alt="2f815423-4aff-486b-aad0-247c102af4b6_removalai_preview" src="https://github.com/user-attachments/assets/d8b53d92-61f5-4964-a4e9-11b543a289d3" />

## Features

- Wireless Remote-Controlled Navigation
- Waterproof 3D Printed Hull
- Camera Integration 
- Arduino-based Smart Control System
- Depth and Leak Sensors
- 6-7 Days Build Timeline

---<img width="1536" height="1024" alt="ChatGPT Image Jul 29, 2025, 04_57_19 PM" src="https://github.com/user-attachments/assets/aa8bd55f-718a-4b47-9c5b-e648d5fd32e5" />
<img width="1907" height="1111" alt="Screenshot 2025-07-29 175733" src="https://github.com/user-attachments/assets/137520f0-b5d7-41b5-9c69-8e5a82a02db1" />

This project aims to build a compact, WiFi-controlled submarine equipped with an ESP32-CAM for live First-Person View (FPV) streaming. It uses brushless waterproof motors for propulsion and servo-controlled fins for steering. The submarine will also log environmental data such as water temperature, depth (via pressure sensor), and motion (via IMU) to an onboard SD card for analysis.

The system is wireless but includes a tether fallback for power or control in case of signal loss. Designed with an acrylic waterproof body, custom 3D-printed parts, and epoxy-sealed electronics, the sub can perform basic underwater maneuvers and real-time monitoring.

🧩 Key Features:
| Feature                | Component Used                 | Purpose                              |
| ---------------------- | ------------------------------ | ------------------------------------ |
| FPV Video Streaming    | ESP32-CAM                      | Real-time video wirelessly           |
| Wireless Control       | ESP32 / Mobile app (future)    | Submarine movement                   |
| Propulsion             | Waterproof Brushless DC Motors | Forward and reverse motion           |
| Steering Control       | SG90 Servo Motors              | Pitch and yaw adjustments            |
| Depth Sensing          | BMP280 / MS5803                | Pressure-based water depth detection |
| Temperature Monitoring | DS18B20 Waterproof Sensor      | Logs water temperature               |
| Orientation Control    | MPU6050 IMU                    | Detect and correct tilt and motion   |
| Data Logging           | SD Card Module + 16GB SD Card  | Stores sensor data                   |
| Waterproof Body        | Acrylic Tube + O-rings + Epoxy | Ensures leak-proof underwater use    |
| Emergency Tether       | Ethernet/Custom Cable          | Power and signal backup              |


📅 6-Day Build Log
📆 Day 1: Research & Sketching
Researched torpedo-style and modular submarines
Studied ballast systems, waterproofing, and RC controls
Sketched a hybrid hull + electronics chamber model
📆 Day 2: Hull Design + Material Planning
Designed initial cylindrical hull with round edges
Planned PLA waterproof printing & internal compartments
Finalized OpenSCAD STL scripting plan
📆 Day 3: Electronics BOM Planning
Selected core components: ESC, Brushless motor, RX-TX
Focused on LiPo safety and compact wiring
Added LEDs and camera slot ideas
📆 Day 4: CAD + 3D Modelling
Designed the hull and rear propeller shaft system
Modeled front dome and rear control fin slots
Prepped STL export files for printing
📆 Day 5: Budgeting & Grant Justification
Created BOM in USD under $200
Wrote README and justification for HackClub grant
Focused on modular design for future upgrades
📆 Day 6: Documentation and Final Touches
Finalized GitHub README
Added diagrams and wiring overview
Cleaned STL files and exported for print test

---

## Tools and Tech Used

- Arduino UNO
- ESC (Electronic Speed Controller)
- LiPo Battery (11.1V 2200mAh)
- 775 DC Motor (2x)
- SG90 Servo (for rudder)
- NRF24L01 Wireless Module
- 3D Printer (PLA filament)
- Fusion 360 / TinkerCAD / OpenSCAD
- Waterproof Sealants
- Miscellaneous wires, tubing, screws

---

## Budget and BOM

Full BOM is in the CSV file: [rc_submarine_bom.csv]

Estimated Total Cost: **$176 USD (~₹14,700)**

---

✅ PHASE-WISE MASTER PLAN (4 Weeks Build)
| **Phase**                           | **Duration** | **Focus**                               | **Goals**                                                                                      |
| ----------------------------------- | ------------ | --------------------------------------- | ---------------------------------------------------------------------------------------------- |
| **Phase 1: Design + Research**      | 3 Days       | Understanding systems & waterproofing   | Finalize design, list all STL parts, check working voltages, sketch wiring, plan inside layout |
| **Phase 2: Procurement**            | 3-4 Days     | Order & collect parts                   | Purchase all electronics, waterproof motors, LiPo, acrylic tube, O-rings, sealants             |
| **Phase 3: Electronics + Code**     | 5 Days       | Soldering + ESP32-CAM + sensors setup   | ESP32-CAM live streaming, test sensors (temp, IMU, pressure), servo testing                    |
| **Phase 4: Mechanical Build**       | 5 Days       | 3D print & waterproof the body          | Print STL mounts, assemble tube + caps, epoxy sealings, mount motor shafts, servo positions    |
| **Phase 5: Integration & Dry Test** | 4 Days       | Fit everything, run tests outside water | Dry test all electronics together, SD logging, camera, motors, IMU orientation                 |
| **Phase 6: Water Test**             | 3 Days       | Shallow testing + tweaks                | Small bucket test first → then pool → test buoyancy, leak check, video, depth sensor           |
| **Phase 7: Final Tuning**           | 2–3 Days     | Add lights, stabilize control           | PID tuning (if needed), tune IMU data, improve signal strength, backup tether setup            |


## License

This project is open-source under the MIT License.

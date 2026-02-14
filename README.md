# Rail-Pulse: On-Board Acoustic Interferometry for Predictive Rail Health Monitoring  
### INGENIUM Season 14 – Engineering Concept Submission

Rail-Pulse is a predictive rail monitoring concept that transforms operational trains into continuous diagnostic platforms.  
The project proposes an Edge-AI–powered acoustic sensing system capable of detecting internal rail fractures in real time during normal train operations.

---

## 🚆 Problem Context

Railway infrastructure worldwide suffers from **Rolling Contact Fatigue (RCF)**—microscopic internal fractures that develop inside steel rails due to repeated stress cycles.

Current inspection methods are limited:

- Ultrasonic inspection trains are expensive and infrequent  
- Manual inspections detect only surface-level damage  
- Maintenance is often schedule-based rather than condition-based  

Undetected internal rail fractures can lead to sudden track failures, derailments, and major economic losses. There is a critical need for **continuous, non-disruptive rail health monitoring**.

---

## 🎯 Project Objective

Rail-Pulse aims to create a system that:

- Detects internal rail fatigue before surface cracks appear  
- Monitors track health continuously using regular trains  
- Enables predictive maintenance instead of scheduled replacement  
- Reduces derailment risk and maintenance costs  

---

## 🧠 Solution Overview

Rail-Pulse uses acoustic fingerprinting of wheel–rail interaction to detect structural anomalies.

### 1️⃣ Sensor Layer
Piezoelectric accelerometers mounted on the train bogie capture high-frequency vibration signals (up to ~20 kHz).

### 2️⃣ Signal Processing
Fast Fourier Transform (FFT) is applied to extract harmonic signatures from wheel–rail interaction.  
Adaptive Noise Cancellation filters engine and ambient noise.

### 3️⃣ Edge AI Classification
A lightweight Convolutional Neural Network processes signals locally on an edge device (e.g., Jetson Nano or Raspberry Pi).  
The model detects abnormal frequency patterns indicating internal fractures.

### 4️⃣ Alert & Visualization
Detected anomalies are tagged with GPS coordinates and transmitted via LoRaWAN/GSM.  
Railway engineers monitor alerts through a cloud dashboard and digital twin visualization.

---

## 🏗 Expected Impact

- **Zero-downtime inspection:** Monitoring happens during normal train operations  
- **Internal defect detection:** Acoustic analysis reveals subsurface fractures early  
- **Cost-efficient maintenance:** Precise location tracking enables targeted repairs  

Primary beneficiaries include railway operators, freight companies, and the travelling public.

---

## 🛠 Proposed Tech Stack

- Piezoelectric accelerometers  
- Edge computing devices (Jetson Nano / Raspberry Pi)  
- FFT signal processing  
- CNN-based anomaly classification  
- LoRaWAN / GSM communication modules  
- Cloud dashboard (React + Firebase concept)

---

## 📊 Project Status

This repository currently contains:

- Concept submission document  
- System architecture design  
- Simulation-based feasibility validation  

The project is in the **Design & Simulation Stage**, with hardware prototyping planned for future phases.

---

## 🔮 Future Development Roadmap

Planned improvements include:

- Federated learning across multiple trains to improve model accuracy  
- Energy harvesting using track vibrations for self-powered sensors  
- Expansion to detect wheel defects in addition to rail fractures  
- Physical prototype deployment on test bogies  

---

## 👤 Author

Rishav Kumar Shrivastava  
KIIT University  

---

## 💡 Vision

Rail-Pulse demonstrates how Edge AI and acoustic sensing can transform railway maintenance from periodic inspection to continuous intelligence, improving safety, efficiency, and infrastructure longevity.

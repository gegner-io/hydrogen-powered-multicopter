# 📘 Project Report: Hydrogen-Powered Multicopter

## 1. Introduction

Modern UAV applications are strongly limited by the energy density of conventional LiPo batteries, resulting in short flight durations and restricted mission capabilities.

This project investigates **hydrogen fuel cells** as an alternative energy source to improve flight endurance and overall system efficiency.

The core objective was to design, build, and evaluate a multicopter system using both:
- 🔋 LiPo battery
- ⚡ Hydrogen fuel cell

and compare their performance under real-world conditions.

---

## 2. Objectives

The project addresses the following key questions:

- How can a multicopter with Pixhawk be designed and integrated with a fuel cell?
- What is the impact of fuel cells on flight performance and endurance?

To answer these, a full system was developed and experimentally evaluated. :contentReference[oaicite:0]{index=0}

---

## 3. System Design

### 3.1 Architecture

The system consists of:

- Quadcopter platform (Tarot 650)
- Pixhawk 4 flight controller
- Hydrogen fuel cell (800W)
- Hybrid battery for peak loads
- Telemetry and ground control system

---

### 3.2 Design Decisions

Key engineering trade-offs:

- ⚖️ Weight vs endurance  
- ⚡ Continuous vs peak power  
- 🔋 Hybrid system necessity  

A quadcopter configuration was chosen to reduce weight and system complexity compared to a hexacopter. :contentReference[oaicite:1]{index=1}

---

## 4. Implementation

### 4.1 Hardware Integration

The system was built from scratch:

- Frame assembly (carbon structure)
- Motor + propeller integration
- Power distribution system
- Fuel cell mounting and integration

Special focus was placed on:
- Low center of mass for stability  
- Safe hydrogen system integration  
- Modular design  

---

### 4.2 Fuel Cell Integration

A hydrogen fuel cell (800W) was integrated as primary energy source.

Key characteristics:

- Max continuous power: **800W**
- Energy capacity: ~**495 Wh usable**
- Requires hybrid battery for load peaks :contentReference[oaicite:2]{index=2}

The hybrid system ensures:
- Stable operation  
- Handling of transient loads  

---

### 4.3 Flight Controller Setup

- Pixhawk 4 with ArduPilot
- Dual power monitoring:
  - Battery
  - Hydrogen tank level
- Failsafe mechanisms for safe operation :contentReference[oaicite:3]{index=3}

---

## 5. Experimental Setup

### 5.1 Test Rig

A custom test bench was developed:

- Aluminum frame structure  
- Fixed drone mount  
- Controlled indoor environment  

This ensured:
- Reproducible measurements  
- No environmental disturbances (wind, weather) :contentReference[oaicite:4]{index=4}

---

### 5.2 Measurement Approach

- Hover tests under varying weights  
- Power consumption monitoring  
- Flight duration estimation  

Key variable:
👉 **Take-off weight vs required power**

---

## 6. Results

### 6.1 Energy System Comparison

| System        | Power Output | Energy Capacity |
|--------------|-------------|----------------|
| Battery      | 6216 W      | 177.6 Wh       |
| Fuel Cell    | 800 W       | 495 Wh         |

:contentReference[oaicite:5]{index=5}

---

### 6.2 Key Findings

- ⚡ Fuel cells provide **significantly higher energy capacity**
- 🔥 Batteries provide **much higher peak power**
- ⚖️ Fuel cell system increases total weight significantly
- 📈 Flight duration depends heavily on power demand and weight

---

### 6.3 Performance Insight

- Fuel cells outperform batteries at **low to moderate power (<800W)**
- Batteries are required for:
  - Take-off
  - Dynamic maneuvers  

👉 Hybrid systems provide the best overall performance.

---

## 7. Discussion

The results clearly show:

- No universal best energy system exists  
- System choice must match mission requirements  

### Fuel Cell Advantages

- Long endurance  
- High energy density  
- Sustainable energy source  

### Limitations

- Limited peak power  
- Complex integration  
- Higher system weight  

---

## 8. Conclusion

The integration of a hydrogen fuel cell into a Pixhawk-based multicopter was successfully demonstrated.

Key outcome:

> Fuel cells significantly extend flight duration but require hybrid support for real-world applications. :contentReference[oaicite:6]{index=6}

This work provides a foundation for future UAV energy systems and highlights the potential of hydrogen technology in aviation.

---

## 9. Future Work

- Advanced hybrid energy management  
- Autonomous mission optimization  
- Simulation (e.g. Unreal Engine)  
- Improved fuel cell control integration  

---

## 📎 Full Thesis

👉 [Full Thesis (PDF)](full-thesis.pdf)
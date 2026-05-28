# ⚙️ Industrial Automation Projects

A collection of PLC and industrial automation projects developed during the **Summer 2025 Industrial Automation Diploma**. All projects are implemented in **CODESYS** using various IEC 61131-3 programming languages, covering real-world automation scenarios from process control to power systems.

---

## 📁 Projects Overview

### 1. 🚗 Automatic Car Washing System
**Language:** Ladder Diagram (LD) & Function Block Diagram (FBD)  
**Tool:** CODESYS  
**Duration:** August 2025

A fully automated car washing system that simulates a real industrial car wash, governed by sensor inputs, timer-controlled operations, and motor-driven actuators.

**How it works:**
- An **entry sensor** detects the vehicle and activates the **conveyor belt**
- The system executes sequential time-based washing stages:
  - Soapy water spraying
  - Brushing
  - Clean water rinsing
  - Drying (1-minute cycle for complete drying)
- An **exit sensor** stops the conveyor automatically after the vehicle clears

**Key Concepts:**
- Sensor-triggered sequential control
- Timer-based stage transitions (TON blocks)
- Conflict prevention through interlock logic
- Multi-language programming in a single CODESYS project

**Skills:** PLC Programming · Ladder Diagram · Function Block Diagram · CODESYS · Process Automation · Timer Control · Sensor Integration

---

### 2. 🦾 Industrial Robotic Arm Pick-and-Place System
**Language:** Structured Text (ST)  
**Tool:** CODESYS  
**Duration:** August 2025

A smart pick-and-place system for an industrial robotic arm that detects objects on a conveyor, picks them up with a gripper, and places them at a target location with precision.

**How it works:**
- A **conveyor sensor** detects incoming objects and triggers the arm sequence
- The arm moves to the object, grips it using calculated gripper force (object weight × safety factor)
- **Linear interpolation** models the arm's trajectory for smooth, continuous motion
- The arm transfers the object to the drop-off point and returns to home position
- A **counter (CTU)** tracks the number of successfully handled objects
- **Emergency stop logic** halts the entire system on abnormal conditions

**Key Concepts:**
- Structured Text for complex algorithmic control
- Linear interpolation for trajectory simulation
- Conveyor speed synchronization with arm cycle time
- Safety and E-stop integration
- Object count tracking for productivity monitoring

**Skills:** PLC Programming · Structured Text · Robotic Kinematics · Motion Control · Safety Logic · CODESYS · Timer & Counter Blocks

---

### 3. ⚡ MV Switchgear Monitoring & Control System
**Language:** Structured Text (ST)  
**Tool:** CODESYS · ModScan/ModSim  
**Duration:** August 2025

A complete automation solution for a **Medium Voltage (MV) Switchgear** system, covering signal acquisition, monitoring, control logic, and Modbus RTU communication — designed using ABB components.

**System Architecture:**
- Hard-wired digital signals for circuit breakers, earth switches, protection relays, and auxiliary systems
- **Modbus RTU** communication over RS485 to acquire soft measurement signals from **Prometer 100** and **NT511** devices
- Real-time data processing: voltages, currents, active/reactive power, frequency, and temperature channels

**Control Logic Implemented:**
- Circuit breaker (CB) interlocking rules
- Protection-based automatic tripping
- Alarm handling and safety conditions
- Manual / remote operation logic

**Validation:**
- All soft signals simulated using **ModScan/ModSim** to verify Modbus register mapping and system behavior

**Deliverables:**
- Complete technical offer document presenting full system architecture
- PLC source code with enum definitions and full sequence-of-operation logic
- Modbus communication validation report

**Skills:** PLC Programming · Modbus RTU · Industrial Communication · MV Switchgear · ABB Components · Structured Text · CODESYS · Signal Mapping · Protection Relays

---

## 🛠️ Tools & Technologies

| Category | Details |
|---|---|
| **PLC IDE** | CODESYS v3.x |
| **Languages** | Ladder Diagram (LD), Function Block Diagram (FBD), Structured Text (ST) |
| **Communication** | Modbus RTU over RS485 |
| **Simulation** | ModSim, ModScan |
| **Hardware Basis** | ABB components (MV switchgear project) |
| **Standard** | IEC 61131-3 |

---

## 📚 Background

These projects were developed as part of an **Industrial Automation Diploma** taken during the summer of 2025. They cover the full range of automation engineering disciplines — from low-level sensor/actuator control to communication protocols and power system protection logic.

---

## 👤 Author

**Abdullah Mohamed**  
Industrial Automation Engineer  
[LinkedIn Profile](https://www.linkedin.com/in/abdullah-mohamed-61801931b/)

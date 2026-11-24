# ⚡ Automatic Power Factor Correction (APFC) System

### Design and Development of an Automatic Power Factor Correction System

**Project Domain:** Electrical Engineering | Power Electronics | Embedded Systems

**Institution:** Jadavpur University, Department of Electrical Engineering

---

## 📌 Project Overview

Power factor is an important parameter in AC electrical systems. A low power factor increases line current, copper losses and voltage drops, reducing the efficiency of electrical installations.

This project focuses on the design and development of a microcontroller-based Automatic Power Factor Correction (APFC) system. The proposed system identifies the phase relationship between voltage and current and uses capacitor-based reactive power compensation to improve the power factor.

The experimental setup uses voltage and current sensing circuits, signal conditioning, DC offset circuits and an Arduino microcontroller.

## 🎯 Objectives

- Understand the fundamental concept of power factor.
- Study resistive, inductive and capacitive loads.
- Develop voltage and current sensing circuits.
- Identify leading and lagging power factor.
- Interface conditioned AC signals with an Arduino.
- Study automatic reactive power compensation using capacitor switching.

## ⚙️ Components Used

| Component | Specification |
|---|---|
| Microcontroller | Arduino Uno R3 |
| Step-down Transformer | 230V / 12-0-12V, 3A |
| Shunt Resistor | 1Ω, 5W |
| Resistive Load | 2 × 10Ω |
| Capacitor | 100µF |
| Inductor | 101.3mH |
| Voltage Divider | 10kΩ and 1.3kΩ |
| DC Offset Supply | 9V Battery |
| Additional Resistors | 300Ω, 1kΩ |
| Coupling Capacitor | 10µF |

## 🔌 Working Principle

The APFC system operates by monitoring the voltage and current signals of the load and determining their phase difference.

The working process involves:

1. **AC Supply:** A step-down transformer provides a 12V AC experimental supply.
2. **Voltage Sensing:** A voltage divider scales down the voltage signal.
3. **Current Sensing:** A 1Ω shunt resistor produces a voltage proportional to load current.
4. **Signal Conditioning:** DC offset circuits shift the sensed AC waveforms into the Arduino's acceptable input range.
5. **Power Factor Identification:** The phase difference between voltage and current is used to identify the nature of the load.
6. **Reactive Power Compensation:** Capacitor-based compensation is considered to reduce lagging reactive power.

## 📐 Theoretical Background

### Power Factor

Power factor is defined as the ratio of active power to apparent power.

**PF = P / S = cos φ**

Where:
- P = Active Power (W)
- S = Apparent Power (VA)
- φ = Phase angle between voltage and current.

### AC Power

- Active Power: P = VI cos φ
- Reactive Power: Q = VI sin φ
- Apparent Power: S = VI

### Reactive Power Compensation

The net reactive power after compensation is:

**Qnet = QL − QC**

Where:
- QL = Inductive reactive power
- QC = Capacitive reactive power

## 🧪 Experimental Calculations

### 1. Resistive Load

Given:
- Load resistance = 20Ω
- Shunt resistance = 1Ω
- Supply voltage = 12V

Total resistance:

Rtotal = 20 + 1 = 21Ω

Load current:

I = 12 / 21 = 0.57A

### 2. Capacitive Load (RC)

Given:
- R = 10Ω
- C = 100µF
- f = 50Hz

Capacitive reactance:

XC = 1 / (2πfC) ≈ 31.83Ω

Impedance magnitude:

|Z| ≈ 33.36Ω

Phase angle ≈ 72.6° leading.

### 3. Inductive Load (RL)

Given:
- R = 10Ω
- L = 101.3mH
- f = 50Hz

Inductive reactance:

XL = 2πfL ≈ 31.83Ω

Impedance magnitude:

|Z| ≈ 33.36Ω

Phase angle ≈ 72.6° lagging.

## 📊 Experimental Observations

- Voltage and current are ideally in phase for a resistive load.
- Current leads voltage in a capacitive RC load.
- Current lags voltage in an inductive RL load.
- The shunt resistor provides a current-proportional voltage signal.
- The voltage divider reduces the sensed voltage.
- The DC offset circuit makes the AC signal suitable for Arduino interfacing.
- Phase difference helps identify the nature of the load power factor.

## ✅ Advantages

- Automatic monitoring of power factor.
- Identification of leading and lagging power factor.
- Reduction in reactive power demand through capacitor compensation.
- Improved utilization of electrical equipment.
- Flexible microcontroller-based control approach.

## 🏭 Applications

- Industrial electrical installations.
- Manufacturing plants.
- Commercial buildings.
- Power distribution systems.
- Motor-driven industrial loads.

## 🔬 Project Scope and Future Development

The project establishes the experimental foundation for microcontroller-based power factor measurement and correction.

Future development can include:
- Complete automatic capacitor bank switching.
- Relay-based capacitor control.
- LCD-based power factor monitoring.
- Testing under different load conditions.
- Further improvement of measurement accuracy.

## 📚 Project Reference

**Project Report:** Design and Development of an Automatic Power Factor Correction System

**Department:** Electrical Engineering

**Institution:** Jadavpur University, Kolkata

**Academic Session:** 2023–2027

## 👨‍💻 Author

**Masud Ali**

B.E. Electrical Engineering

Jadavpur University

- GitHub: [@alimasudali](https://github.com/alimasudali)
- LinkedIn: [Masud Ali](https://www.linkedin.com/in/masud-ali-4268643b5/)

---

⭐ *Exploring Power Electronics, Embedded Systems and Electrical Engineering Innovations.*

**Note:** Arduino source code is not included in this repository because it is not currently available. The documentation is based on the project report.

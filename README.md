# 🔴 Sigma Embedded — AUTOSAR DEM Simulators

> Interactive tools to visualize and understand AUTOSAR DEM behavior in real time

---

## 🚀 Overview

This repository provides a set of **interactive web-based simulators** for the AUTOSAR Diagnostic Event Manager (DEM).

Instead of only reading specifications, you can **experiment and visualize** how debounce algorithms and DTC states evolve.

---

## 🧩 Simulators

### 🟠 Counter-Based Debounce
- Implements `DemDebounceCounterBased`
- Configurable increment/decrement steps
- Counter range: **-127 ↔ +127**
- State transitions:
  - `PREPASSED → PASSED`
  - `PREFAILED → FAILED`
- DTC storage & healing visualization

---

### 🟢 Time-Based Debounce
- Implements `DemDebounceTimeBased`
- Adjustable thresholds:
  - FAILED timer
  - PASSED timer
- Real-time signal simulation (press & hold)
- Accurate ECU-like timing behavior

---

### 🔵 Full DTC Status Byte (8-bit)
- Based on **ISO 14229-1 / AUTOSAR SWS_Dem**
- Includes:
  - `testFailed`
  - `pendingDTC`
  - `confirmedDTC`
  - `warningIndicatorRequested`
- Features:
  - Drive cycle (DCY)
  - Fault confirmation threshold
  - Aging mechanism
  - DTC clearing

---

## 🎯 Purpose

AUTOSAR DEM is often difficult to understand from documentation alone.

This project allows you to:
- 👁️ Visualize behavior
- 🧠 Understand transitions
- ⚙️ Experiment with parameters
- 🚀 Learn faster through interaction

---

## 🧠 What You’ll Learn

- Counter-based vs Time-based debounce
- DTC lifecycle (pending → confirmed → cleared)
- Drive cycle behavior
- Full 8-bit DTC status logic

# co-FDII-tool

**Integrated tool for the identification of cyber-attacks in PV power plants**  
Developed under the **COCOON European project**

This repository contains an integrated tool designed for detecting and analyzing potential cyber-attacks targeting photovoltaic (PV) power plants. The dataset is organized into three main folders, each representing a different scenario of system behavior and attack conditions.

## Folder Structure

### 1. `Scenarios` - Base Case
- Contains the **normal operation data** of the PV plant.
- All measurements are genuine and represent standard operating conditions.
- **Residuals are zero**, indicating no anomalies or attacks are present.

### 2. `Dummy_attacks` - Basic Attack Scenario
- Simulates **simple manipulation** of the system measurements.
- Specifically, the **active power measurement of LV0102** is altered by multiplying the measured value by **1.2** (i.e., a 20% increase).
- Useful for testing basic anomaly detection capabilities.

### 3. `Smart_attacks` - Advanced Attack Scenario
- The **voltage measurement at node LV0102** is altered by multiplying the measured value by **0.98** (i.e., a 2% decrease).
- Involves more sophisticated attacks where multiple measurements are manipulated to evade detection.
- The following measurements are modified:
  - **Measurement 5**: `Q_LV0102` (Reactive power at LV0102)
  - **Measurement 10**: `U_LV0103` (Voltage at LV0103)
  - **Measurement 15**: `I_LV0201_MV0201` (Current from LV0201 to MV0201)
  - **Measurement 20**: `P_LV0203` (Active power at LV0203)
  - **Measurement 25**: `Q_POIMV_MV0101` (Reactive power at POIMV_MV0101)

These modifications simulate coordinated attacks aiming to mislead monitoring systems while maintaining internal consistency.

---

## Applications
- Detection of stealthy cyber-attacks in PV systems
- Evaluation of fault detection and isolation algorithms
- Benchmarking intrusion detection systems in energy infrastructures
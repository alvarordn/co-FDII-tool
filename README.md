# co-FDII-tool

**Integrated tool for the identification of cyber-attacks in PV power plants**  
Developed under the **COCOON European project**

This repository contains an integrated tool designed for detecting and analyzing potential cyber-attacks targeting photovoltaic (PV) power plants. The dataset is organized into four main folders, each representing a different scenario of system behavior and attack conditions.

## Folder Structure

### 1. `Scenarios` - Base Case
- Contains the **normal operation data** of the PV plant.
- All measurements are genuine and represent standard operating conditions.
- **Residuals are zero**, indicating no anomalies or attacks are present.

### 2. `dummy_0_5` 
- Simulates **simple manipulation** of the system measurements.
- Specifically, the **active power measurement of LV0102** is altered by multiplying the measured value by **0.5** (i.e., a 50% decrease).
- Useful for testing basic anomaly detection capabilities.

### 3. `dummy_1_2` 
- Simulates **simple manipulation** of the system measurements.
- Specifically, the **active power measurement of LV0102** is altered by multiplying the measured value by **1.2** (i.e., a 20% increase).
- Useful for testing basic anomaly detection capabilities.

### 4. `dummy_3` 
- Simulates **simple manipulation** of the system measurements.
- Specifically, the **active power measurement of LV0102** is altered by multiplying the measured value by **0.5** (i.e., a 300% increase).
- Useful for testing basic anomaly detection capabilities.


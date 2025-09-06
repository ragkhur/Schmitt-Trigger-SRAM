# Schmitt-Trigger Based Low Power SRAM (45-nm CMOS)

This repository documents the design and analysis of an **11T Schmitt-Trigger Based SRAM cell** implemented in **45-nm CMOS technology**.  
The project was developed as part of the **Digital CMOS VLSI Design (VLS 503)** course at IIIT Bangalore.

---

## Project Overview
- Implemented an **11T Schmitt-Trigger SRAM cell** to improve **Static Noise Margin (SNM)** and minimize read disturbance compared to the conventional 6T SRAM cell.  
- Utilized **separate read/write ports** to enhance stability and eliminate read–write coupling issues.  
- Conducted **PVT (Process-Voltage-Temperature) simulations** and **Monte Carlo analysis**, validating robustness under fabrication and environmental variations.  
- Benchmarked against 6T SRAM architecture, achieving **significant energy per bit reduction** and better noise resilience.

---

##  Tech Stack
- **45-nm CMOS PDK**  
- **Cadence Virtuoso** – Schematic/Layout Design  
- **Synopsys HSPICE** – Circuit Simulation & SNM Analysis  
- **Matlab/Python** – Data visualization of simulation results  

*(Note: Design files are hosted on institute systems and cannot be publicly shared. This repo provides the report, results, and documentation.)*

---

## Key Results

### Static Noise Margin (SNM) Comparison
- Conventional **6T SRAM** (baseline):  
  ![6T SNM Read 0](results/snm_6t_read0.png)  
  ![6T SNM Read 1](results/snm_6t_read1.png)  

- Proposed **11T Schmitt-Trigger SRAM**:  
  ![11T SNM Read 0](results/snm_11t_read0.png)  
  ![11T SNM Read 1](results/snm_11t_read1.png)  
  ![11T SNM Hold 0](results/snm_11t_hold0.png)  
  ![11T SNM Hold 1](results/snm_11t_hold1.png)  
  ![11T SNM Write 1](results/snm_11t_write1.png)  

---

### PVT Analysis (Process, Voltage, Temperature Corners)
- Hold SNM across PVT:  
  ![Hold SNM Typ](results/pvt_hold_typ.png)  
  ![Hold SNM Worst](results/pvt_hold_worst.png)  

- Write/Read SNM across PVT:  
  ![Write SNM Worst](results/pvt_write_worst.png)  

---

## Repository Contents
- `report/` – Final project report & reference papers  
- `results/` – Plots and tables from simulations  

---

## References
1. Oruga et al., *Schmitt-Trigger Based Low Power SRAM in 45-nm CMOS*, IEEE, 2023.  
2. IIIT Bangalore VLS 503 Project Report (2024).  

---

## Authors  
- Raghav Khurana
- Divyansh Kumar
- Puneet Kalyan Upadrasta  
- Abu Saleh Khan  
- Shruti Singh  
- Keerthana B  


---


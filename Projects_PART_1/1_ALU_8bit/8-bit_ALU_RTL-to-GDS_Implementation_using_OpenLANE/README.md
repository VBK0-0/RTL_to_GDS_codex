# 📘 8-bit ALU RTL-to-GDS Implementation using OpenLANE

---

## 🔹 Overview  
This project implements an **8-bit Arithmetic Logic Unit (ALU)** in Verilog and takes it through a complete **RTL-to-GDSII flow** using open-source tools.  
The ALU performs basic arithmetic and logical operations and demonstrates the **digital ASIC implementation process** from RTL to final layout.  

---

## 🔹 Objectives  
- Write RTL design in Verilog.  
- Functionally verify with Icarus Verilog + GTKWave.  
- Perform logic synthesis using Yosys.  
- Run floorplanning, placement, CTS, and routing using OpenLANE.  
- Perform DRC/LVS checks with Magic & Netgen.  
- Run static timing analysis (STA) with OpenSTA.  
- Generate final GDSII layout.  

---

## 🔹 Tools Used  
- **Simulation**: Icarus Verilog, GTKWave  
- **Synthesis**: Yosys  
- **Backend**: OpenLANE, Magic, KLayout  
- **Verification**: OpenSTA (timing), Netgen (LVS)  
- **Technology Node**: Sky130 PDK  

---

## 🔹 Design Details  
- **Top Module**: `alu8.v`  
- **Clock Frequency / Period**: 100 MHz / 10 ns  
- **Operations Supported**: Add, Subtract, AND, OR, XOR, Shift Left, Shift Right  
- **I/O Ports**:  
  - Inputs: `a[7:0]`, `b[7:0]`, `op[2:0]`  
  - Outputs: `result[7:0]`, `carry`  

---

## 🔹 Project Workflow  

1. **RTL Design**  
   - Wrote Verilog code for ALU.  

2. **Functional Verification**  
   - Simulated with Icarus Verilog.  
   - Verified results with GTKWave waveforms.  

3. **Logic Synthesis (Yosys)**  
   - Generated gate-level netlist.  
   - Extracted cell count, area, and timing report.  

4. **Physical Design (OpenLANE)**  
   - Floorplanning  
   - Placement  
   - Clock Tree Synthesis (CTS)  
   - Routing  

5. **Sign-off Checks**  
   - DRC with Magic.  
   - LVS with Netgen.  
   - STA with OpenSTA.  

6. **Final Layout**  
   - Generated GDSII file.  

---

## 🔹 Results  

- **Simulation Waveforms:**  
  ![Simulation Waveform](./results/simulation_waveform.png)  

- **Synthesis Report (Yosys):**  
  - Cell Count: **XXX**  
  - Area: **XXXX µm²**  
  - Critical Path Delay: **X ns**  

- **Layout Screenshots:**  
  - Floorplan: ![Floorplan](./results/floorplan.png)  
  - Placement: ![Placement](./results/placement.png)  
  - Routed Layout: ![Routed Layout](./results/routed_layout.png)  

- **Final GDSII:**  
  - [Download GDS File](./results/alu8.gds)  

---

## 🔹 Challenges Faced & Learnings  
- Resolved DRC violations during routing.  
- Learned about clock tree balancing in CTS.  
- Understood STA reports and fixed timing issues.  

---

## 🔹 Future Improvements  
- Add pipelining for performance improvement.  
- Optimize power using clock gating.  
- Extend ALU to 16-bit or 32-bit.  

---

## 🔹 References  
- [OpenLANE Documentation](https://github.com/The-OpenROAD-Project/OpenLane)  
- [SkyWater 130nm PDK](https://github.com/google/skywater-pdk)  
- [Yosys Open Synthesis Suite](http://www.clifford.at/yosys/)  

---

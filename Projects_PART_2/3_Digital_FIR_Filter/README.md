# 📘 FIR Filter RTL-to-GDS

## 🔹 Overview
This project implements a **Finite Impulse Response (FIR) Filter** in Verilog and performs RTL-to-GDSII using open-source ASIC tools.

## 🔹 Objectives
- Implement FIR RTL using shift registers and multipliers.
- Verify filter behavior with testbench.
- Run backend flow for layout.
- Generate timing & area reports.

## 🔹 Tools Used
- Icarus Verilog, GTKWave
- Yosys
- OpenLANE, Magic
- OpenSTA
- PDK: Sky130

## 🔹 Design Details
- Top Module: `fir.v`
- Inputs: `clk`, `reset`, `x_in`
- Output: `y_out`

## 🔹 Workflow
1. RTL design.  
2. Testbench with sample inputs.  
3. Synthesis (Yosys).  
4. Backend flow (OpenLANE).  
5. STA and final GDS.  

## 🔹 Results
- Verified FIR outputs ✅  
- Timing & area reports ✅  
- Layout image ✅  

## 🔹 Learnings
- DSP block design in RTL.  
- Understanding multipliers & adders.  

## 🔹 Future Improvements
- Parameterized filter order.  
- Optimize for power.  

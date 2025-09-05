# 📘 8-bit Counter with Clock Gating RTL-to-GDS

## 🔹 Overview
This project implements an **8-bit synchronous counter** with clock gating for low power. It is synthesized and placed using open-source ASIC tools.

## 🔹 Objectives
- Implement counter with clock gating logic.
- Verify functionality in simulation.
- Run RTL-to-GDS flow in OpenLANE.
- Highlight power savings.

## 🔹 Tools Used
- Icarus Verilog, GTKWave
- Yosys
- OpenLANE, Magic
- OpenSTA
- PDK: Sky130

## 🔹 Design Details
- Top Module: `counter8.v`
- Inputs: `clk`, `reset`, `enable`
- Outputs: `count[7:0]`

## 🔹 Workflow
1. RTL coding in Verilog.  
2. Functional verification.  
3. Synthesis (Yosys).  
4. Physical design in OpenLANE.  
5. STA and DRC/LVS checks.  

## 🔹 Results
- Simulation waveform ✅  
- Gated clock reduces unnecessary toggles ✅  
- Clean GDSII layout ✅  

## 🔹 Learnings
- Clock gating for power optimization.  
- Handling clock constraints in STA.  

## 🔹 Future Improvements
- Extend to up/down counter.  
- Add programmable reset value.  

## 🔹 References
- [Yosys](http://www.clifford.at/yosys/)  

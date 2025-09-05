# 📘 OpenRAM SRAM Integration Project

## 🔹 Overview
This project uses **OpenRAM** to generate a custom SRAM macro and integrates it into a small SoC design.

## 🔹 Objectives
- Generate SRAM using OpenRAM.
- Integrate SRAM into RTL design.
- Run backend flow in OpenLANE.
- Verify LVS & timing.

## 🔹 Tools Used
- OpenRAM
- Yosys
- OpenLANE, Magic, Netgen
- OpenSTA
- PDK: Sky130

## 🔹 Workflow
1. Run OpenRAM to generate SRAM.  
2. Add SRAM to RTL design.  
3. Synthesis.  
4. Backend flow.  
5. DRC/LVS clean GDSII.  

## 🔹 Results
- Custom SRAM block ✅  
- Integrated SoC layout ✅  

## 🔹 Learnings
- Memory compiler basics.  
- Integration of hard macros.  

## 🔹 Future Improvements
- Explore larger SRAMs.  
- Optimize timing closure.  

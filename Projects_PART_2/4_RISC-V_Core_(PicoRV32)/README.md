# 📘 RISC-V Core RTL-to-GDS

## 🔹 Overview
This project implements the **PicoRV32 RISC-V core** using the open-source flow, taking it from RTL to GDSII.

## 🔹 Objectives
- Download & integrate PicoRV32 RTL.
- Perform synthesis with Yosys.
- Run OpenLANE flow for layout.
- Verify timing closure.

## 🔹 Tools Used
- Yosys
- OpenLANE, Magic
- OpenSTA
- PDK: Sky130

## 🔹 Workflow
1. Clone PicoRV32 RTL.  
2. Set up CSV/config in OpenLANE.  
3. Run synthesis & backend flow.  
4. Check STA & reports.  
5. Final GDSII.  

## 🔹 Results
- Successful RTL-to-GDS flow ✅  
- Layout screenshots ✅  
- Reports on area & timing ✅  

## 🔹 Learnings
- Implementing CPU cores.  
- Handling larger RTL designs.  

## 🔹 Future Improvements
- Add peripherals.  
- Explore multi-core design.  

# 📘 SPI Protocol Controller RTL-to-GDS

## 🔹 Overview
This project implements a **Serial Peripheral Interface (SPI) Controller**. The design supports master-slave communication and is implemented end-to-end using open tools.

## 🔹 Objectives
- Design SPI master & slave RTL modules.
- Simulate & verify communication.
- Synthesize and implement physical design.
- Generate GDSII layout.

## 🔹 Tools Used
- Icarus Verilog, GTKWave
- Yosys
- OpenLANE, Magic, KLayout
- OpenSTA
- PDK: Sky130

## 🔹 Design Details
- Top Module: `spi_top.v`
- Ports: `clk`, `mosi`, `miso`, `sclk`, `cs`

## 🔹 Workflow
1. Write SPI RTL.  
2. Verify master-slave data transfer.  
3. Run synthesis.  
4. Backend in OpenLANE.  
5. DRC/LVS clean GDSII.  

## 🔹 Results
- Functional verification ✅  
- Successful data exchange ✅  
- Layout screenshots ✅  

## 🔹 Learnings
- Digital protocol design in RTL.  
- Handling synchronous serial links.  

## 🔹 Future Improvements
- Add multi-slave support.  
- Implement advanced clock division.  

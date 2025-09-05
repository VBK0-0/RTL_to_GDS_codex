# 📘 UART Controller RTL-to-GDS

## 🔹 Overview
This project implements a **UART (Universal Asynchronous Receiver/Transmitter)** including TX, RX, and baud generator modules. The design is taken from RTL to layout.

## 🔹 Objectives
- Write UART RTL modules in Verilog.
- Functionally verify transmission & reception.
- Perform synthesis & place and route.
- Generate final GDSII.

## 🔹 Tools Used
- Icarus Verilog, GTKWave
- Yosys
- OpenLANE, Magic
- OpenSTA, Netgen
- PDK: Sky130

## 🔹 Design Details
- Top Module: `uart_top.v`
- Inputs: `clk`, `reset`, `rx`
- Outputs: `tx`, `data_out`

## 🔹 Workflow
1. RTL coding for TX, RX, Baud generator.  
2. Testbench simulation.  
3. Synthesis & reports.  
4. OpenLANE flow for layout.  
5. DRC/LVS clean GDSII.  

## 🔹 Results
- Simulation waveforms ✅  
- Correct serial data exchange ✅  
- GDSII layout ✅  

## 🔹 Learnings
- Protocol-level RTL design.  
- Handling async signals.  

## 🔹 Future Improvements
- Add parity/error detection.  
- Implement FIFO buffer.  

## 🔹 References
- [UART Protocol Basics](https://en.wikipedia.org/wiki/Universal_asynchronous_receiver-transmitter)  

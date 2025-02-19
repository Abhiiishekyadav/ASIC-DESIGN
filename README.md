## Digital Design Flow using Cadence-GPDK 90nm  

This repository contains design files and scripts for ASIC design flow using the GPDK 90nm technology node. The workflow is divided into front-end synthesis and back-end physical design using industry-standard EDA tools.

### Repository Structure  

- GENUS_COMPILER  
  - Contains scripts and files for logic synthesis using Cadence Genus Compiler.  
  - Converts RTL code (Verilog/VHDL) into a gate-level netlist.  
  - Performs technology mapping and timing optimization.  

- RTL_COMPILER  
  - Another synthesis tool used for RTL-to-GDSII flow.  
  - Generates a gate-level netlist with constraints applied.  
  - Focuses on area, power, and timing optimization.  

- INNOVUS_COMPILER  
  - Contains files for physical design using Cadence Innovus.  
  - Takes the synthesized netlist and performs placement, clock tree synthesis (CTS), and routing.  
  - Ensures Design Rule Check (DRC) and Layout vs. Schematic (LVS) compliance.  

### Technology Used  
- Technology Node: GPDK 90nm  
- Tools Used:  
  - Front-End: Genus Compiler, RTL Compiler  
  - Back-End: Innovus Compiler  

### Design Flow Summary  
1. Front-End (Logic Synthesis) 
   - RTL Design (Verilog/VHDL)  
   - Synthesis using Genus/RTL Compiler  
   - Constraints application (timing, area, power)  

2. Back-End (Physical Design)  
   - Netlist import into Innovus  
   - Floorplanning, Placement, CTS, Routing  
   - DRC/LVS Checks and final GDSII generation  

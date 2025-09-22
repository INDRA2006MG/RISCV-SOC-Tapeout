# RISCV-SOC-Tapeout
Open-source RISC-V System-on-Chip (SoC) design targeting tapeout, including RTL, verification, synthesis, and physical design flows. 

## Program Description
This initiative spotlights the RISC-V SoC chip tapeout program, jointly organized by VLSI System Design (VSD) and IIT Gandhinagar (IITGN). Spanning 20 weeks, the program provides practical exposure to a full tapeout cycle for a RISC‑V Reference SoC, making use of Synopsys tools and the SCL180 nm PDK. As part of India’s Semiconductor Mission, the program is dedicated to developing skilled VLSI engineers with a focus on real-world fabrication at national foundries (SCL). By fostering technical expertise, this effort is set to drive the next era of innovation in the country’s VLSI ecosystem(https://www.vlsisystemdesign.com/soc-labs/)

## Highlights:
+ Functional Validation
+ Custom IP Integration
+ Full-Chip Gate-Level Simulation
+ Physical Design Preparation
+ Full-Chip Implementation
+ Signoff & Tapeout
+ Post-Silicon Validation
## Outcomes
1. Able to design a complete RISC-V based SoC and Tapeout the same.

# WEEK 0 

## Environment + RTL sim basics

**Task 1: Create GitHub repo** 
+(https://github.com/INDRA2006MG/RISCV-SOC-Tapeout/edit/main/README.md)
  
**Task 2: Tool Installation**
  ## Tools installation instructions
 + Oracle virtual machine link : https://www.virtualbox.org/wiki/Downloads
   
**System Check**
+ 6GB RAM, 50 GB HDD
+ Ubuntu 20.04+
+ 4vCPU 
![system info](https://github.com/INDRA2006MG/RISCV-SOC-Tapeout/blob/main/Pictures/IMG_20250920_233832.jpg)
**Yosys**
```
$ sudo apt-get update
$ git clone https://github.com/YosysHQ/yosys.git
$ cd yosys
$ sudo apt install make               # If make is not installed
$ sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
$ make config-gcc
# Yosys build depends on a Git submodule called abc, which hasn't been initialized yet. You need to run the following command before running make
$ git submodule update --init --recursive
$ make 
$ sudo make install
```

**iVerilog**
```
$ sudo apt-get update
$ sudo apt install gtkwave
```
**GTKWAVE**
```
$ sudo apt-get update
$ sudo apt install gtkwave
```

# 🔧 Virtual FPGA with JIT Compiler
This project implements a Virtual FPGA (Field Programmable Gate Array) environment powered by a JIT (Just-In-Time) Compiler backend. It simulates key hardware components like LUTs, Flip-Flops, and Registers, while integrating LLVM-based JIT compilation for runtime execution of hardware logic described in a high-level language.
A software simulation of an FPGA environment, integrated with a Just-In-Time (JIT) compiler using LLVM. This project allows users to define and execute digital circuits virtually, simulating hardware behavior with high performance.

## 📌 Project Objectives
- Emulate core FPGA logic components (LUTs, Flip-Flops, Registers).
- Dynamically generate and execute logic using LLVM-based JIT compilation.
- Provide a modular, extensible simulator for educational and research purposes.
- Bridge the gap between hardware-level simulation and software-level control.


## 🧩 Key Features
- ✅ **LUT Simulation**: Define custom combinational logic using Lookup Tables.
- 🔁 **Flip-Flops & Registers**: Simulate sequential logic and clocked behavior.
- ⚙️ **LLVM-Based JIT**: Convert virtual circuit logic to native machine code at runtime.
- 🔄 **Cycle-Accurate Simulation**: Step-by-step simulation for accurate timing analysis.
- 🧪 **Unit Tests**: Example and test cases to validate functionality of components.


## 🛠️ Architecture Overview
+-----------------------+
|  Circuit Description  |
+----------+------------+
           |
           v
+-----------------------+
|   Simulation Engine   |<------+
|  (LUTs, FFs, Regs)    |       |
+----------+------------+       |
           |                    |
           v                    |
+-----------------------+       |
|    LLVM JIT Engine    |       |
|  (Code Generation)    |       |
+----------+------------+       |
           |                    |
           v                    |
+-----------------------+       |
|   Execution Backend   |<------+
+-----------------------+


## 📂 Folder Structure
FPGA/
├── include/             # Header files for all hardware components
├── fpga_simulator.py/                 # Core logic and simulator source files
├── jit_executor.py/                   # Test cases and sample circuit definitions
├── jit_codegen.py/                    # Compiled output 
└── gui.py                             # User Interface            
└── README.md                          # Project documentation


## 📈 Future Enhancements
- 🖥️ GUI interface for drag-and-drop circuit building
- 📜 Verilog/HDL input parser
- 📊 Real-time logical problem handling
- 📦 More hardware components (RAM, Multiplexers, etc.)
- 🔬 Benchmarking and performance visualization

# Custom 8-Bit Microprocessor

This repository contains the complete design, architecture, and implementation details of a custom-built 8‑bit microprocessor. The goal of the project is to design a Turing-complete 8‑bit CPU with a 16‑bit address bus, a compact custom ISA, and a simulation-ready microarchitecture.

![alt text](<docs/Screenshot (1241).png>)

## 🚀 Key Features

- 8‑bit data bus
- 16‑bit address bus (64 KiB address space)
- Turing‑complete instruction set (work in progress)
- Custom ISA: Arithmetic, Logical, Memory, Branch, and Special instructions
- Microarchitecture with control signals and cycle‑accurate timing states
- Simulation-ready for Logisim Evolution
- Stack support (PUSH / POP), branching, I/O, and memory access (some parts pending implementation)

---

## 📐 Architecture Overview

- **ALU Operations:** ADD, SUB, AND, OR, XOR, NOT, SHL, SHR
- **Immediate Ops:** ADDI, SUBI, ANDI, ORI, MOVI
- **Memory Instructions:** LD, ST, MOV, PUSH, POP
- **Control Flow:** JMP, JZ, JNZ, JC, CALL, RET
- **Special:** CMP, TEST

You can refer to the instruction table for complete opcode mapping.
There are many instruction that are not yet completed that i am currently working

---

## 🖥 Microarchitecture

- Control Unit design with micro-operations
- Clock cycle–based timing diagrams
- ALU module
- Register file design
- Memory interface

![alt text](<Screenshot (1237).png>)
---
![alt text](<docs/Screenshot (1240).png>)

![alt text](<docs/Screenshot (1239).png>)

## 🧪 Simulation

You can run the CPU in Logisim Evolution using the provided circuit (usually sim/logisim.circ or sim/cpu.circ). The ROM is pre-populated with example programs — edit the ROM contents to run your own programs.

Supported simulator:

- **Logisim Evolution**

---

## ▶️ How to Run (quick)

Open the CPU.circ file in Logisim Evolution.

Load or edit the ROM (some ROMs are plain .hex files you can import into the ROM component).

Click the clock input or enable the simulator clock. Use the clock tick/step for single-step execution.

Slow the clock down if you want to visually follow each micro-operation.

Tip: Use the single‑step/tick feature in Logisim Evolution to observe register changes and control signal timings.

---

## 🛠 Editing the ROM / Programs

ROMs in the repository are usually provided as .hex or as the content configured in the ROM component inside Logisim.

To test programs: write assembly, assemble it to machine code (hex), and paste the hex into the ROM or replace the ROM file referenced by the circuit.

I plan to provide an assembler that translates the custom assembly into a ROM file.

---

## 🧩 Contributing

Contributions are welcome!

Open issues for bugs and feature requests

Add example programs under examples/

If you submit a PR with new instructions or microcode, please include a brief test program demonstrating the behavior.

Suggested branch naming: feature/<short-desc> or fix/<short-desc>

---

## 🔭 Future Work

Build a custom assembler/compiler that outputs ROM files from human-readable assembly

Implement more I/O instructions and memory-mapped peripherals

Expand instruction set and microcode optimizations

Add automated tests and simulation scripts to run sample programs

---

## 📬 Contact / Author

Created by Preetham — feel free to open issues or PRs for improvements.

I attempted to build this project entirely on my own, with only minimal reference from others(including chatgpt),while trying to keep it as simple as possible, as I wanted to challenge myself and understand every part of the design. Because of that, there may be areas that can be improved — suggestions and contributions are welcome!

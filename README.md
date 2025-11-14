# Custom 8-Bit Microprocessor

This repository contains the complete design, architecture, and implementation details of my custom-built 8-bit microprocessor.  
The goal of this project is to design a Turing-complete 8-bit CPU with a 16-bit address bus, a simple ISA, microarchitecture.

---

## 🚀 Features

- 8-bit data bus
- 16-bit address bus
- Turing-complete instruction set(building in process)
- Fully custom ISA (Arithmetic, Logical, Memory, Branch, and Special instructions)
- Microarchitecture with control signals and timing states
- Simulation-ready for Logisim Evolution
- Supports stack operations (PUSH, POP), branching, I/O, and memory access(to be implemented yet)

---

## 📐 Architecture Overview

- **ALU Operations:** ADD, SUB, AND, OR, XOR, NOT, SHL, SHR
- **Immediate Ops:** ADDI, SUBI, ANDI, ORI, MOVI
- **Memory Instructions:** LD, ST, MOV, PUSH, POP
- **Control Flow:** JMP, JZ, JNZ, JC, CALL, RET
- **Special:** CMP, TEST

You can refer to the instruction table for complete opcode mapping.

---

## 🖥 Microarchitecture

- Control Unit design with micro-operations
- Clock cycle–based timing diagrams
- ALU module
- Register file design
- Memory interface

---

## 🧪 Simulation

This project can be run in:

- **Logisim Evolution**

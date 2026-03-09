# Verilog 4-bit Calculator ALU

This project implements a simple 4-bit digital calculator using Verilog HDL.  
The calculator can perform arithmetic operations such as addition, subtraction, multiplication, and division.

The design is based on a modular digital architecture including registers, multiplexers, decoders, and an Arithmetic Logic Unit (ALU).

## Project Overview

The system operates on 4-bit inputs and produces results up to 8-bit output values.

The calculator supports the following operations:

- Addition
- Subtraction
- Multiplication
- Division

It also includes status signals such as:

- done
- div_by_zero
- negative

## Architecture

The system is composed of multiple hardware modules:

### Decoder
Selects which register (A or B) should receive input data.

### Multiplexers
Used to route data between different parts of the datapath.

### Registers
Two 4-bit registers store the input operands.

### Full Adder
Implements 1-bit addition with carry.

### Ripple Carry Adder
Constructed using four 1-bit full adders.

### Adder/Subtractor
Performs addition or subtraction using two's complement logic.

### Arithmetic Logic Unit (ALU)
Executes arithmetic operations:

- ADD
- SUB
- MUL
- DIV

### Datapath
Connects all modules together and manages data flow between registers and the ALU.

## Tools Used

- Verilog HDL
- ModelSim (simulation)
- Digital Logic Design principles

## Simulation

Each module was tested using dedicated Verilog testbenches.  
Waveforms were analyzed in ModelSim to verify correct operation.

Modules tested include:

- decoder
- multiplexers
- registers
- full adder
- ripple carry adder
- ALU
- datapath

## Project Structure

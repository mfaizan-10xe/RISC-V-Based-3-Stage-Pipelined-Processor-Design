# RISC-V Based 3-Stage Pipelined Processor Core

This repository contains the SystemVerilog implementation of a 3-Stage Pipelined RISC-V processor core capable of executing instructions with I, R, B, S, J, and U formats. The processor core design adheres to the RISC-V instruction set architecture (ISA) and is intended for educational and academic purposes.

## Overview

The RISC-V processor core is designed to execute instructions in a pipeline, providing deterministic performance. It supports the following instruction formats:

- **I-Type Instructions:** Instructions with an immediate operand, typically used for arithmetic and logical operations.
- **R-Type Instructions:** Register-to-register instructions, often used for arithmetic and logical operations.
- **B-Type Instructions:** Branch instructions, facilitating conditional branching based on comparison results.
- **S-Type Instructions:** Store instructions, used for storing data from a register to memory.
- **J-Type Instructions:** Jump instructions, facilitating unconditional jumps to different parts of the program.
- **U-Type Instructions:** Upper immediate instructions, used for loading immediate values into registers.

The processor core architecture includes modules for instruction fetch, instruction decode, execution, memory access, and write-back stages. Each stage is designed to handle a specific aspect of instruction execution, ensuring efficient and accurate operation.

## Features

- **Pipeline Execution:** Instructions are executed in a pipeline, providing deterministic performance.
- **Support for RISC-V ISA:** Implements a wide range of instruction formats, covering most common operations in RISC-V programs.
- **Modular Design:** Processor architecture is modular, allowing for easy understanding, debugging, and modification.
- **CSR Support:** Integrating privilege support by implementing basic Control and Status Registers (CSRs) for trap handling.

## Simulation

Simulation of the RISC-V processor core can be performed using the ModelSim simulator. 

## Usage

To use the RISC-V processor core design, instantiate the `Three_stage_Pipeline.sv` module in your SystemVerilog project. Connect appropriate inputs and outputs to interface with external memory, peripherals, and control logic as needed.

## Acknowledgments

- This project was inspired by the need for a simple yet functional RISC-V processor core suitable for educational purposes.
- Special thanks to the RISC-V community for providing extensive documentation and resources on RISC-V ISA and microarchitecture.


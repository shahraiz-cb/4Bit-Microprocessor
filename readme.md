# 4-bit Microprocessor

This is a 4-bit microprocessor that I built for a class project. It is a 4-bit processor with 8 instructions, 16 4-bit registers. It is capable of performing basic arithmetic as well as branching and looping. The simulation has been done in Proteus.

README file for 4-bit Microprocessor

# Introduction:

This document provides an overview of the 4-bit microprocessor architecture and its features. This microprocessor is designed for applications that require basic arithmetic and logical operations.

# Architecture:

The microprocessor consists of four main components: an arithmetic and logic unit (ALU), a program counter (PC), a memory unit, and a control unit. The ALU performs arithmetic and logical operations on data stored in the memory unit. The PC keeps track of the memory address of the current instruction being executed. The memory unit stores both program instructions and data. The control unit manages the flow of data between the ALU, PC, and memory unit.

# Instruction Set:

The instruction set consists of 9 instructions, each represented by a 4-bit opcode. The instructions include basic arithmetic including NOP, LDI, ADD, INC,JUMP, BRNE, SUB, MOV, and OUT. There are also instructions for conditional branching.

# Memory Unit:

The Memory Unit consists of a 16x4-bit memory array, which is used to store data and instructions. The memory unit supports both read and write operations, allowing data to be read from and written to memory.

# Limitations:

The microprocessor has a limited instruction set and can only perform simple operations.
The microprocessor has limited memory capacity and can only handle small programs.

# Examples:

For running the bin files provided, make sure to burn "InsDec.bin" and "IncDec_1.bin" files to the "INSDEC" and "INSDEC_1" EEPROMs respectively.

## Sample Code 1:

Loops over the code to increment the contents of R0 and outputs it on the PORT.

```
LDI R0, 0x00
OUT R0
INC R0
JMP 0x00
```

In order to run the code, burn sampleCode1.bin and sampleCode1_1.bin to the "CODEMEM" "CODEMEM_1" EEPROMs in proteus respectively.

## Sample Code 2:

```
LDI R0, 0x05
LDI R1, 0x05
OUT R0
OUT R1
SUB R0, R1
OUT R0
```

Corresponding files for this code are "addTest.bin" and "addTest_1.bin"

# Conclusion:

The 4-bit microprocessor is a low-cost, low-power solution for basic arithmetic and logical operations. Its small size and low power consumption make it ideal for battery-powered devices and other applications that require a compact, energy-efficient solution.

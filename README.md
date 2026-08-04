# Airport-Terminal-Tram-Controller

# Custom Single-Cycle Microprocessor – Airport Terminal Tram Controller
## Overview
This project implements a custom-designed single-cycle microprocessor that executes an Airport Terminal Tram Controller using a Finite State Machine (FSM). Rather than implementing the controller purely in software, the project focuses on designing the underlying processor hardware responsible for executing the controller's instructions.

The processor, datapath, and control logic were built from scratch using Digital Logic. Every major hardware component—including the ALU, control unit, multiplexers, registers, memory interface, and program counter—was designed and integrated into a functioning processor capable of executing the FSM.

---

## Project Objectives

- Design a custom single-cycle processor
- Implement a complete datapath and control unit
- Design a functional Arithmetic Logic Unit (ALU)
- Interface instruction memory and RAM
- Execute an Airport Terminal Tram Controller using an FSM
- Verify processor operation through simulation

---

## Airport Terminal Tram Controller

The application running on the processor is an Airport Terminal Tram Controller modeled as a Finite State Machine.
The tram progresses through numbered terminal states while enforcing directional and operational constraints.
### Example State Progression
Upward operation:
```
2 → 4 → 6 → 8 → 10
```
Downward operation:
```
10 → 8 → 6 → 4 → 2
```
Only one direction may be active at any time.
State transitions occur only after required operating conditions are satisfied (such as doors being closed), preventing invalid transitions and ensuring deterministic system behavior.

---

## Processor Architecture
The processor consists of individually designed hardware modules, including:

- Arithmetic Logic Unit (ALU)
- Control Unit
- Instruction Decoder
- Program Counter
- Address Generator
- Register File
- RAM Interface
- Multiplexers
- Incrementer
- Add/Subtract Logic
- Data Bus Routing

Each component was designed independently and then integrated into the complete processor.

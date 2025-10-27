# Computer Architecture Lab: What I Did, What I Understood, and Viva Preparation

**Student:** Muhammad Bilal  
**Class:** BSCS V-B  
**Subject:** Computer Architecture Lab

---

## Assignment Explanation: What Was Done and Learned

### Lab 1: Basic Logic Gates
- Implemented AND, OR, NOT, NAND, and NOR gates in Verilog
- Simulated these gates using ModelSim; analyzed outputs with testbenches
- Learned how these gates form the foundation of all digital logic circuits and how their truth tables dictate their behavior

### Lab 2: Adder Circuits
- Designed and simulated Half Adder and Full Adder circuits
- Half Adder: Performed binary addition of two bits; outputs SUM and CARRY. Logic: SUM = A ⊕ B, CARRY = A AND B
- Full Adder: Added three bits (A, B, Cin), outputs SUM and CARRY. Logic: SUM = A ⊕ B ⊕ Cin, CARRY = (A AND B) OR (B AND Cin) OR (A AND Cin)
- Confirmed designs matched expected truth tables using testbenches

### Lab 3: Subtractor Circuits, Multiplexer & Demultiplexer
- Designed and simulated Half Subtractor and Full Subtractor circuits
- Half Subtractor: Produced difference and borrow for two bits
- Full Subtractor: Managed three inputs (A, B, Borrow-in), and produced difference and borrow-out
- Built and tested 2x1 and 4x1 multiplexers for data selection, demultiplexers for data routing
- Understood how multiplexers enable selection between inputs while demultiplexers distribute a signal to multiple outputs

---

## What I Understood
- Digital systems start with basic gates, which are combined to create functional circuits for arithmetic and logic processing
- Adders and subtractors are essential for performing binary arithmetic; multiplexers and demultiplexers control data flow
- Verilog allows us to describe and simulate these circuits before hardware implementation; ModelSim provides the visualization for verification
- Testbenches are crucial for validating design correctness against theoretical truth tables

---

## Possible Viva Questions

### Fundamental Concepts
- What is the role of a testbench in ModelSim?
- Why are AND, OR, and NOT gates called the basic gates?
- How is a NAND gate universal?

### Adder and Subtractor Circuits
- What is the difference between a half adder and a full adder?
- Explain the logic expressions for SUM and CARRY in a full adder.
- How do half subtractor and full subtractor circuits differ?
- What is the function of a borrow in subtraction circuits?

### Multiplexers and Demultiplexers
- How does a 2x1 multiplexer work? What about a 4x1?
- Describe the role of select lines in a multiplexer.
- What is the main application of a demultiplexer in digital systems?

### Verilog and Simulation
- Why do we use Verilog for digital design?
- What is the advantage of simulating circuits in ModelSim?
- How do you debug a faulty simulation result?

### Application and Understanding
- What are the real-world applications of adder and subtractor circuits?
- In what scenarios would you use a multiplexer?
- How does combinational logic differ from sequential logic?

---

## Viva Questions and Answers for Computer Architecture Lab Fundamental Concepts

### Q: What is the role of a testbench in ModelSim?
A testbench in ModelSim is used to simulate and verify the behavior of your digital circuits by applying a series of test inputs and observing the outputs. It ensures that your Verilog code works correctly by automating the testing process and comparing actual results with expected results.​

### Q: Why are AND, OR, and NOT gates called the basic gates?
AND, OR, and NOT gates are called basic gates because they perform primary logical operations and from these, all other complex gates and functions can be constructed. They are the foundational elements for building digital circuits.​

## Q: How is a NAND gate universal?
A NAND gate is considered universal because any digital circuit or logic function can be implemented using only NAND gates. This is due to its ability to recreate AND, OR, and NOT functions by appropriate combinations.​

## Adder and Subtractor Circuits
### Q: What is the difference between a half adder and a full adder?
A half adder adds two single-bit numbers and produces a sum and a carry. A full adder adds three bits (including a carry-in) and produces a sum and a carry-out. Full adders are used to construct multi-bit addition by connecting them in series.​

## Q: Explain the logic expressions for SUM and CARRY in a full adder.

SUM: 
A
⊕
B
⊕
Cin
A⊕B⊕Cin, where 
⊕
⊕ denotes XOR

CARRY: 
(
A
⋅
B
)
+
(
B
⋅
Cin
)
+
(
A
⋅
Cin
)
(A⋅B)+(B⋅Cin)+(A⋅Cin)​

### Q: How do half subtractor and full subtractor circuits differ?
A half subtractor subtracts two single bits and outputs the difference and borrow. A full subtractor handles subtraction of three bits (including borrow-in), producing difference and borrow-out, allowing chain subtraction for multi-bit numbers.​

### Q: What is the function of a borrow in subtraction circuits?
Borrow indicates when subtraction cannot be completed without taking one from a higher place value bit. It is needed in multi-bit binary subtraction to maintain calculation accuracy.​

## Multiplexers and Demultiplexers
Q: How does a 2x1 multiplexer work? What about a 4x1?
A 2x1 multiplexer selects one of two input signals based on a single select line. A 4x1 multiplexer selects one out of four inputs using two select lines, routing the selected signal to the output. Multiplexers are used for data selection in digital systems.​

### Q: Describe the role of select lines in a multiplexer.
Select lines determine which input is passed to the output. For example, in a 4x1 multiplexer, two select lines (S1, S0) decide which input (I0–I3) is routed to the output.​

### Q: What is the main application of a demultiplexer in digital systems?
Demultiplexers distribute a single input signal to one of several outputs, based on select lines. They are essential for applications where one data source needs to be sent to multiple destinations.​

## Verilog and Simulation
### Q: Why do we use Verilog for digital design?
Verilog is a hardware description language that allows designers to model, simulate, and verify digital circuits before physically building them. It enables quick debugging and performance testing.​

### Q: What is the advantage of simulating circuits in ModelSim?
Simulation in ModelSim allows for visualization of circuit behavior, easy debugging, and verification of correctness before real-world implementation, saving time and cost.​

### Q: How do you debug a faulty simulation result?
Debugging involves checking the Verilog code for syntax or logic errors, reviewing the testbench inputs, analyzing waveforms in ModelSim, and ensuring correct connections and signal values.​

## Application and Understanding
### Q: What are the real-world applications of adder and subtractor circuits?
Adders and subtractors are used in arithmetic operations within CPUs, calculators, DSPs, and any device requiring numerical computation. They’re part of arithmetic logic units and data processing blocks.​

### Q: In what scenarios would you use a multiplexer?
Multiplexers are useful wherever digital data routing and selection are needed—such as memory address selection, data bus management, and communication lines in processors.​

### Q: How does combinational logic differ from sequential logic?
Combinational logic output depends only on present inputs. Sequential logic circuits have memory, meaning outputs depend on present inputs and previous states, which is essential for counters, registers, and state machines.​

## Tips for Viva Preparation
- Memorize logic expressions and truth tables for each circuit
- Review Verilog code structure for each component
- Practice explaining the purpose of each gate/circuit in your own words
- Be ready to discuss simulation results and common debugging strategies

---

**This document covers all major aspects studied in the labs and provides enough detail to prepare for both the assignment and viva.**

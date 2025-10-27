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

## Tips for Viva Preparation
- Memorize logic expressions and truth tables for each circuit
- Review Verilog code structure for each component
- Practice explaining the purpose of each gate/circuit in your own words
- Be ready to discuss simulation results and common debugging strategies

---

**This document covers all major aspects studied in the labs and provides enough detail to prepare for both the assignment and viva.**

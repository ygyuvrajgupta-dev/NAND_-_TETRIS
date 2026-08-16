# Lab 1: Digital Logic & ALU Design

## Overview

This project is part of **Lab 1: Digital Logic & ALU Design**. The objective of this lab is to design, implement, and verify foundational combinational logic chips using **Nand2Tetris HDL** and the **Nand2Tetris Hardware Simulator/Web IDE**.

The lab focuses on understanding digital logic design, NAND universality, Boolean logic, data routing, 16-bit logic operations, multi-way multiplexing/demultiplexing, and eventually the complete Hack ALU.

All implemented chips were tested using their corresponding Nand2Tetris test scripts. The simulation results were verified against the provided comparison files.

---

## Tools Used

* **Nand2Tetris Web IDE**
* **Nand2Tetris Hardware Simulator**
* **Nand2Tetris HDL**
* **GitHub** for documentation and submission evidence

---

## Objectives

The main objectives of this laboratory work are:

* Understand the fundamentals of combinational digital logic.
* Demonstrate how complex logic can be constructed from basic gates.
* Understand the concept of NAND universality.
* Implement Boolean logic gates using HDL.
* Implement 16-bit logic gates.
* Design multiplexers and demultiplexers.
* Implement multi-way multiplexers and demultiplexers.
* Verify each implementation using simulation test scripts.
* Analyze and verify simulation outputs using the provided comparison files.
* Develop the logic required for the final Hack ALU.

---

## Implementation and Verification

The following chips have been implemented and successfully verified in the Nand2Tetris Web IDE.

| No. | Chip      | Status |
| --: | --------- | ------ |
|   1 | Not       |  PASS |
|   2 | And       |  PASS |
|   3 | Or        |  PASS |
|   4 | Xor       |  PASS |
|   5 | Mux       |  PASS |
|   6 | DMux      |  PASS |
|   7 | Not16     |  PASS |
|   8 | And16     |  PASS |
|   9 | Or16      |  PASS |
|  10 | Mux16     |  PASS |
|  11 | Or8Way    |  PASS |
|  12 | Mux4Way16 |  PASS |
|  13 | Mux8Way16 |  PASS |
|  14 | DMux4Way  |  PASS |
|  15 | DMux8Way  |  PASS |

Each test produced the successful simulation result:

**"Simulation successful: The output file is identical to the compare file."**

---

## 1. Not Gate

The `Not` chip performs logical negation.

* Input `0` produces output `1`.
* Input `1` produces output `0`.

The implementation was tested successfully using the Nand2Tetris test script.


---

## 2. And Gate

The `And` chip produces `1` only when both inputs are `1`.

The implementation was verified for all required input combinations.


---

## 3. Or Gate

The `Or` chip produces `1` when at least one of its inputs is `1`.

The implementation was successfully verified using the provided test script.


---

## 4. Xor Gate

The `Xor` chip produces `1` when the two input values are different.

The implementation was constructed using NAND-based logic and successfully verified.



---

## 5. Mux

The `Mux` (Multiplexer) selects one of two inputs based on the `sel` control signal.

* `sel = 0` → output follows `a`
* `sel = 1` → output follows `b`

The implementation successfully passed the simulation.

---

## 6. DMux

The `DMux` (Demultiplexer) routes one input to one of two outputs according to the selection signal.

The implementation was successfully tested for both selection states.


---

## 7. Not16

`Not16` performs bitwise logical negation on a 16-bit input.

Each of the 16 input bits is processed independently.


---

## 8. And16

`And16` performs bitwise AND operation on two 16-bit inputs.

The implementation was tested using multiple 16-bit input patterns.


---

## 9. Or16

`Or16` performs bitwise OR operation on two 16-bit inputs.

The implementation successfully passed all provided test cases.

---

## 10. Mux16

`Mux16` is a 16-bit multiplexer that selects between two 16-bit input values.

The selection is controlled by the `sel` input.

---

## 11. Or8Way

`Or8Way` performs OR operation across eight input bits.

The output becomes `1` if any of the eight input bits is `1`.

---

## 12. Mux4Way16

`Mux4Way16` selects one of four 16-bit inputs using a 2-bit selection signal.

The four possible selections are:

* `00` → `a`
* `01` → `b`
* `10` → `c`
* `11` → `d`

The implementation was successfully verified.

---

## 13. Mux8Way16

`Mux8Way16` selects one of eight 16-bit input values using a 3-bit selection signal.

All eight selection combinations were tested successfully.

---

## 14. DMux4Way

`DMux4Way` routes a single input to one of four output lines based on a 2-bit selection signal.

The implementation was successfully verified for all four selection combinations.

---

## 15. DMux8Way

`DMux8Way` routes a single input to one of eight outputs using a 3-bit selection signal.

The implementation was successfully tested for all eight selection combinations.

---

## Progress Summary

### Completed and Verified

* [x] Not
* [x] And
* [x] Or
* [x] Xor
* [x] Mux
* [x] DMux
* [x] Not16
* [x] And16
* [x] Or16
* [x] Mux16
* [x] Or8Way
* [x] Mux4Way16
* [x] Mux8Way16
* [x] DMux4Way
* [x] DMux8Way


## Conclusion

This laboratory work demonstrates the implementation and verification of fundamental digital logic components using **Nand2Tetris HDL**. The completed chips were tested in the Nand2Tetris Web IDE, and their simulation outputs successfully matched the provided comparison files.

The work provides the foundation for constructing arithmetic circuits and the final **Hack ALU**, which combines logic and arithmetic operations using control signals.

---


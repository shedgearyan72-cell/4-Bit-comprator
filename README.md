# 4-Bit-comprator
# 4-Bit Comparator — CircuitVerse

A digital logic project that compares two 4-bit binary numbers.

## Inputs

- A3 A2 A1 A0
- B3 B2 B1 B0

## Outputs

- A > B
- A = B
- B > A

## Architecture

The project uses four reusable 1-bit comparator subcircuits.

Each 1-bit comparator produces:

- A > B
- A = B
- B > A

The four comparator blocks are combined using priority logic, where the
most significant differing bit determines the result.

## 1-Bit Comparator Logic

### A > B

A AND NOT B

### B > A

B AND NOT A

### A = B

XNOR

## Technologies

- CircuitVerse
- Digital Logic Gates
- Combinational Logic

## Learning

This project helped me understand:

- AND, OR, NOT, XOR, XNOR, NAND
- Truth tables
- Subcircuits
- Multi-bit comparison
- Priority logic
- Combinational circuit design

# Full Adder

A Full Adder is a combinational digital circuit that performs the addition of three 1-bit binary inputs.

Unlike a Half Adder, a Full Adder can also accept a carry from a previous addition.

## Inputs

- A
- B
- Cin (Carry In)

## Outputs

- SUM
- CARRY OUT

## Logic Used

The Full Adder is built using:

- 2 Half Adders
- 1 OR Gate

### First Half Adder

The first Half Adder adds A and B.

It produces:

- Intermediate Sum
- Carry 1

### Second Half Adder

The Intermediate Sum from the first Half Adder is added with Cin.

It produces:

- Final SUM
- Carry 2

### OR Gate

The two carry outputs are connected to an OR Gate.

This produces the final CARRY OUT.

## Logic Equations

SUM = A XOR B XOR Cin

CARRY OUT = (A AND B) OR (Cin AND (A XOR B))

## Truth Table

| A | B | Cin | SUM | CARRY OUT |
|---|---|-----|-----|-----------|
| 0 | 0 |  0  |  0  |     0     |
| 0 | 0 |  1  |  1  |     0     |
| 0 | 1 |  0  |  1  |     0     |
| 0 | 1 |  1  |  0  |     1     |
| 1 | 0 |  0  |  1  |     0     |
| 1 | 0 |  1  |  0  |     1     |
| 1 | 1 |  0  |  0  |     1     |
| 1 | 1 |  1  |  1  |     1     |

## Components Used

- 3 Input Switches
- 2 Half Adder Subcircuits
- 1 OR Gate
- 2 Output LEDs

## Working

The Full Adder works in three stages:

1. The first Half Adder adds A and B.
2. The second Half Adder adds the intermediate SUM with Cin.
3. The OR Gate combines both carry outputs to produce CARRY OUT.

For example:

1 + 1 + 1 = 11

Therefore:

SUM = 1  
CARRY OUT = 1

The two outputs together represent the binary result `11`.

## Circuit Structure

A + B → Half Adder 1
              ↓
        Intermediate SUM
              ↓
       + Cin → Half Adder 2
              ↓
             SUM

Half Adder 1 Carry ──┐
                     ├── OR → CARRY OUT
Half Adder 2 Carry ──┘

## Testing

The circuit was tested with all 8 possible combinations of A, B, and Cin.

All outputs were verified successfully in CircuitVerse.


## Tool Used

CircuitVerse

## Next Step

The Full Adder can be combined with other Full Adders to create a multi-bit binary adder.

Full Adder → 4-bit Ripple-Carry Adder → ALU → CPU

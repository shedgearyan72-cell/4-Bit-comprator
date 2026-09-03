# Half Adder

A Half Adder is a combinational digital circuit that performs the addition of two 1-bit binary numbers.

## Inputs

- A
- B

## Outputs

- SUM
- CARRY

## Logic Used

The Half Adder is built using two logic gates:

### XOR Gate
The XOR gate produces the SUM output.

SUM = A XOR B

### AND Gate
The AND gate produces the CARRY output.

CARRY = A AND B

## Truth Table

| A | B | SUM | CARRY |
|---|---|-----|-------|
| 0 | 0 |  0  |   0   |
| 0 | 1 |  1  |   0   |
| 1 | 0 |  1  |   0   |
| 1 | 1 |  0  |   1   |

## Components Used

- 2 Input Switches
- 1 XOR Gate
- 1 AND Gate
- 2 Output LEDs

## Working

Both inputs A and B are connected to the XOR and AND gates.

The XOR gate calculates the SUM, while the AND gate calculates the CARRY.

For example:

1 + 1 = 10

Therefore:

SUM = 0  
CARRY = 1

The circuit was tested with all four possible input combinations and verified successfully.

## Circuit

![Half Adder Circuit](circuit.png)

## Tool Used

CircuitVerse

## Next Step

The Half Adder is used as a building block for the Full Adder.

Half Adder → Full Adder → 4-bit Ripple-Carry Adder → ALU → CPU

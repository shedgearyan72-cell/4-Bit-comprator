# 4-bit Subtractor

A 4-bit binary subtractor built in CircuitVerse using four Full Adder subcircuits.

This circuit performs subtraction using the two's complement method:

**A - B = A + (~B) + 1**

Instead of creating a separate subtractor from scratch, the circuit reuses the Full Adder designed earlier.

---

## 🧠 How It Works

The subtractor uses the two's complement method.

For every bit of B:

1. Pass B through a NOT gate to obtain `~B`.
2. Add `~B` to A using four Full Adders.
3. Set the initial Carry-In (`CIN`) to `1`.
4. The carry from each Full Adder is passed to the next Full Adder.

Therefore:

```text
A - B = A + (~B) + 1

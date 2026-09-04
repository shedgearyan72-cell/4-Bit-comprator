# 4-bit ALU (Add/Sub)

A 4-bit Arithmetic Logic Unit built in CircuitVerse.

This ALU performs two arithmetic operations:

- `OP = 0` → Addition (`A + B`)
- `OP = 1` → Subtraction (`A - B`)

The circuit combines XOR gates with four Full Adders to create a single Add/Subtract unit.

---

## 🧠 How It Works

The ALU uses an operation control input called `OP`.

### OP = 0 → Addition

When `OP = 0`:

```text
B XOR 0 = B
CIN = 0

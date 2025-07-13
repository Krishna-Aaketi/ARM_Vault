
# 📚 CPU Instruction Structure – Explained Step by Step

---

## 🔧 What is a CPU Instruction?

A **CPU instruction** is a single command given to the processor. It's like a line of code in the CPU's native language, telling it to:

- Do a calculation (e.g., add or subtract)
- Move data (e.g., from memory to register)
- Make a decision (e.g., jump if zero)

It’s part of the **instruction set** defined by the CPU’s architecture (like ARM, MIPS, x86, etc.).

---

## 🧱 Structure of an Instruction (Simplified)

Every instruction generally has 3 key parts:

| Part          | Role                                 | Example from `ADD R1, R2, R3`  |
|---------------|--------------------------------------|--------------------------------|
| **Opcode**    | Operation to perform (like a verb)   | `ADD` → tells CPU to add       |
| **Operands**  | Input data (registers or memory)     | `R2`, `R3` → values to be added|
| **Destination**| Where to store the result (register)| `R1` → holds the result        |

---

## 🔷 1. Opcode – What to do

### ✅ Meaning:
The **action or instruction type**.  
Tells the CPU what operation to perform (e.g., add, move, load, store).

### 🧠 Think of it like:
> A verb in a sentence → it defines the **action**.

### 💬 Example:
```asm
ADD R1, R2, R3
```
Here, `ADD` is the **opcode**.

### 🔩 Common Opcodes:

| Opcode | Meaning         |
|--------|------------------|
| ADD    | Add values       |
| SUB    | Subtract         |
| MOV    | Move/copy data   |
| LDR    | Load from memory |
| STR    | Store into memory|

---

## 🔷 2. Operands – What to operate on

### ✅ Meaning:
The **inputs** or **data sources**, usually **registers** or **memory locations**.

### 🧠 Think of it like:
> Nouns in a sentence → the things being acted upon.

### 💬 Example:
```asm
ADD R1, R2, R3
```
Operands are `R2` and `R3`.

### 🔎 Operand Types:

| Type        | Example   | Description                        |
|-------------|-----------|------------------------------------|
| Register    | R2, R3    | Fast storage inside CPU            |
| Immediate   | #5        | Constant number                    |
| Memory      | [R0]      | Data from memory address in R0     |

---

## 🔷 3. Destination – Where to store result

### ✅ Meaning:
Tells the CPU **where to save the output** of the operation, often a **register**.

### 🧠 Think of it like:
> The **target or result** of the action.

### 💬 Example:
```asm
ADD R1, R2, R3
```
Destination is `R1`.

✅ This means: `R1 = R2 + R3`

---

## 🧾 Summary Table

| Part        | What it Does                     | Example in `ADD R1, R2, R3` |
|-------------|----------------------------------|------------------------------|
| **Opcode**  | Operation type                   | ADD                          |
| **Operands**| Input values                     | R2, R3                       |
| **Destination** | Output/result register         | R1                           |

---

## 👀 Bonus Example Instructions

| Instruction        | Description                                      |
|--------------------|--------------------------------------------------|
| MOV R0, #10        | Load 10 into R0                                  |
| SUB R2, R2, #1     | Decrement R2 by 1                                |
| STR R3, [R1]       | Store R3’s value into memory at address in R1    |
| LDR R4, [R1]       | Load from memory pointed by R1 into R4           |

---

## 🧠 Why This Matters

| Role             | Impact                                      |
|------------------|----------------------------------------------|
| **Opcode**        | Decides the CPU operation                   |
| **Operands**      | Provides input data                         |
| **Destination**   | Sets where the result goes                  |
| **Clear Structure**| Allows efficient pipeline design           |


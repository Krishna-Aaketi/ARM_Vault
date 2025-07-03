# Day 1: RISC vs CISC + History of ARM

---

## ✅ Part 1: What is RISC?

**RISC = Reduced Instruction Set Computer**  
A CPU design that uses a **small set of simple instructions** that execute very fast.

### 🟢 Key Features of RISC:
- Each instruction takes **1 clock cycle** to execute (ideally)
- Focuses on **simplicity and speed**
- Uses **many general-purpose registers**
- Fewer instruction formats → **easier decoding**
- **Load/Store architecture** → only `LOAD` and `STORE` access memory

### 🛠️ Example Instructions (RISC):
```asm
MOV R0, #5      ; Load 5 into R0  
ADD R1, R0, #2  ; Add 2 to R0 and store in R1  
STR R1, [R2]    ; Store R1 value into memory pointed by R2
```
### ✅ Advantages of RISC:

- Faster execution (due to simple instructions)
- Easier pipelining
- Low power consumption
- Simple hardware → cheaper

---

## ✅ Part 2: What is CISC?

**CISC = Complex Instruction Set Computer**  
A CPU design that uses **many complex instructions**, some of which may take **multiple cycles**.

---

### 🔴 Key Features of CISC:

- Large instruction set (e.g., 200+ instructions)
- One instruction can do **multiple things** (e.g., load + add + store)
- Fewer registers
- Hardware is **complex and power-hungry**

---

### 🛠️ Example Instructions (CISC – x86):

```asm
MOV AX, [BX]    ; Move from memory to AX directly  
ADD AX, 10      ; Add 10 to AX
```
### ❌ Disadvantages of CISC:

- More complex CPU design  
- Slower execution for some instructions  
- Harder to pipeline

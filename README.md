# Day 1: RISC vs CISC + History of ARM

## Part 1: What is RISC?

**RISC = Reduced Instruction Set Computer**  
A CPU design that uses a **small set of simple instructions** that execute very fast.

### Key Features of RISC:
- Each instruction takes **1 clock cycle** to execute (ideally)
- Focuses on **simplicity and speed**
- Uses **many general-purpose registers**
- Fewer instruction formats → **easier decoding**
- **Load/Store architecture** → only `LOAD` and `STORE` access memory

### Example Instructions (RISC):
```asm
MOV R0, #5      ; Load 5 into R0  
ADD R1, R0, #2  ; Add 2 to R0 and store in R1  
STR R1, [R2]    ; Store R1 value into memory pointed by R2
```
### Advantages of RISC:

- Faster execution (due to simple instructions)
- Easier pipelining
- Low power consumption
- Simple hardware → cheaper

## Part 2: What is CISC?

**CISC = Complex Instruction Set Computer**  
A CPU design that uses **many complex instructions**, some of which may take **multiple cycles**.

### Key Features of CISC:

- Large instruction set (e.g., 200+ instructions)
- One instruction can do **multiple things** (e.g., load + add + store)
- Fewer registers
- Hardware is **complex and power-hungry**

### Example Instructions (CISC – x86):

```asm
MOV AX, [BX]    ; Move from memory to AX directly  
ADD AX, 10      ; Add 10 to AX
```
### Disadvantages of CISC:

- More complex CPU design  
- Slower execution for some instructions  
- Harder to pipeline

### Part 3: RISC vs CISC – Comparison Table
```
Q)What is the difference between RISC and CISC?
| Feature                  | RISC (ARM)             | CISC (x86)              |
|--------------------------|------------------------|--------------------------|
| Instruction Set          | Small and simple       | Large and complex        |
| Clock Cycles per Instr.  | Mostly 1               | Multiple                 |
| Memory Access            | Only by load/store     | Can access during ALU ops|
| Register Usage           | More general registers | Fewer registers          |
| Power Consumption        | Low                    | High                     |
| Code Size                | Larger (more lines)    | Smaller                  |
| Execution Speed          | High                   | Moderate                 |
| Used In                  | Mobiles, Embedded      | PCs, Laptops             |
```
### Part 4: History of ARM

| Year        | Event                                                  |
|-------------|--------------------------------------------------------|
| 1983        | ARM project started by Acorn Computers for BBC Micro   |
| 1985        | First ARM processor: ARM1                              |
| 1990        | ARM Holdings Ltd. formed                               |
| 1993–2000   | ARM7/ARM9 dominate embedded devices                    |
| 2004        | Cortex series launched (M, A, R)                       |
| 2010        | ARM becomes dominant in smartphones                    |
| 2020        | Apple shifts Macs to ARM-based M1 chip                 |
| 2021+       | ARM enters data centers, AI, ML, automotive            |

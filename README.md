# DAY 1: What is ARM Architecture? (Introduction + History + Basics)

## Goal of Day 1

Understand:

- What is CPU Architecture what is does
- What is ARM   
- Why ARM is used  
- Where ARM is used  
- Difference between ARM vs others  
- History & evolution


## 1.What is a CPU Architecture?
```
**CPU architecture** = design or blueprint of how a processor works.

It defines:

- How instructions are executed  
- How data is stored/moved  
- How the control unit and ALU operate  

**Examples**: x86, MIPS, RISC-V, ARM
```
## How Instructions Are Executed

### Definition:
An **instruction** is a small command like `add`, `load`, `store`, or `compare`.  
The **CPU reads** these instructions from memory and **executes** them step by step.

### Phases of Instruction Execution (Instruction Cycle):

1. **Fetch** – CPU gets the instruction from memory.
2. **Decode** – CPU understands what the instruction is.
3. **Execute** – CPU performs the task (e.g., adding numbers).
4. **Write-back** – Result is stored in a register or memory.

---

### Example (ADD Instruction)

```assembly
ADD R0, R1, R2    ; R0 = R1 + R2

```
## 2. How Data is Stored/Accessed (Memory Movement)

### Memory Types:

| Memory Type   | Description                                                 |
|---------------|-------------------------------------------------------------|
| **Registers** | Small, fast storage inside the CPU (e.g., R0, R1)           |
| **RAM**       | Main memory; larger but slower than registers               |
| **Cache**     | Medium-speed memory between RAM and CPU; improves access time |

---

### Instructions for Moving Data:

- `LDR` → **Load** data from memory into a register
- `STR` → **Store** data from a register into memory

These are called **load/store instructions** and are key to RISC architectures like ARM.

---

### Example:

#### Given:

```text
R1 = 0x2000  
Memory[0x2000] = 99


## 2.What is ARM?
```
- **ARM** stands for **Advanced RISC Machine**  
- It is a **RISC-based processor architecture**  
- Created by a UK company named **ARM Holdings**  
- **ARM Holdings licenses** the design, doesn't manufacture chips  

**Examples of users**: Apple, Samsung, Qualcomm all use ARM cores.
```
## 3.What is RISC?
```
| Feature     | RISC (like ARM)        | CISC (like x86)         |
|-------------|------------------------|--------------------------|
| Instructions| Few & simple           | Many & complex           |
| Speed       | Fast                   | Slower                   |
| Power       | Low power              | High power               |
| Usage       | Mobile, IoT, embedded  | Laptops, desktops        |

```
## 4.Short History of ARM
```
| Year | Event                                   |
|------|-----------------------------------------|
| 1983 | First ARM chip by Acorn Computers       |
| 1990 | ARM Holdings founded                    |
| 2001 | ARM7 used in Nokia phones               |
| 2010 | Cortex-M series → Embedded systems      |
| 2020 | Apple M1/M2 → ARM in laptops            |
```
## 5.Where is ARM Used?
```
| Device           | Example                     | ARM Chip            |
|------------------|-----------------------------|----------------------|
| Smartphones      | iPhone, Samsung Galaxy       | Cortex-A             |
| Embedded Systems | Smartwatch, Fitness bands    | Cortex-M             |
| Automotive       | Car ECU, infotainment        | Cortex-R             |
| IoT Devices      | Smart bulb, WiFi switches    | Cortex-M0/M4         |
| Laptops/Tablets  | MacBook M1, iPad             | Apple ARM-based SoCs |
```
## 6.ARM vs x86 Comparison
```
| Feature        | ARM              | x86             |
|----------------|------------------|-----------------|
| Type           | RISC             | CISC            |
| Power          | Low              | High            |
| Instruction Set| Simple           | Complex         |
| Used in        | Phones, IoT, MCUs| PCs, Servers    |
| Cost           | Cheaper          | Costly          |
```
## 7.ARM Naming Confusion Simplified
```
| Name Type     | Meaning                                  |
|---------------|------------------------------------------|
| ARM7, ARM9    | Old families (legacy)                    |
| Cortex-M      | For Microcontrollers (STM32, LPC)        |
| Cortex-R      | For Real-time systems (automotive)       |
| Cortex-A      | For Application Processors (phones)      |
| Neoverse      | For Servers/Data Centers                 |
```
## 8.Why is ARM so Popular?
```
- Low power usage  
- High performance per watt  
- Licensable → others can customize (e.g. Apple M1)  
- Small size → fits in embedded devices  
- Growing ecosystem (STM32, Raspberry Pi, Android)
```
## 9.Quick Recap
```
- ARM = RISC-based, low power CPU architecture  
- Used everywhere: phones, smartwatches, MCUs, laptops  
- Designed by ARM Holdings  
- Famous for Cortex-M, Cortex-A families  
- Different from x86 (used in PCs)
```

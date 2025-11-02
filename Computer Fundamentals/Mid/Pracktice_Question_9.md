### **Practice Midterm Question 09 (Challenge Version)**

**Daffodil International University**
**Department of Software Engineering**
**Midterm Examination, Spring 2025**
**Course Code: SE 111; Course Title: Computer Fundamentals**

**Time: 1 Hour 30 Mins**
**Marks: 25**

**Answer ALL Questions**
---

**1. a)** A museum is restoring two computational artifacts. The first is a cabinet from a 1960s **transistor-based** computer, containing schematics for a "Central Processor" that executes instructions sequentially from a magnetic tape—a process where the **Control Unit** follows a rigid, non-interactive program path. The second artifact is the silicon wafer of a modern multi-core processor, designed for a high-end workstation that runs dozens of applications simultaneously under a multitasking OS, where the **Control Unit** must constantly switch contexts based on OS commands. [Marks-3]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Analyze the fundamental role and operational differences of the CPU's Control Unit (CU) and Arithmetic Logic Unit (ALU) when comparing the "one job at a time" batch processing model of the 1960s computer versus the dynamic, interactive multitasking model of the modern processor.**

**b)** A CPU architect is finalizing the design of a new high-performance core. A critical decision is the on-die memory allocation. A portion of the silicon is reserved for an array of storage cells that hold the operands and results of the *exact* instruction currently being executed by the ALU. The adjacent, much larger portion is reserved for a high-speed buffer that holds copies of data and instructions from RAM that are *likely to be needed next*. [Marks-3]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&-**nbsp;&nbsp;Identify these two types of on-die memory. Compare them based on their precise function in the CPU instruction cycle, their relative size and access speed, and why both are necessary for modern performance.**

**c)** Execute the following complex number system conversions, showing all intermediate steps: [Marks-9]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; i) Convert **421₅** to its equivalent number in Base 15 (Use A=10, B=11...F=14).
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ii) Convert **11010.011₂** to its equivalent number in Base 4.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; iii) Convert **213.875₁₀** to its equivalent number in Base 2 (Binary).

---

**2. a)** The XNOR (Exclusive-NOR) gate, which outputs '1' only when its inputs are identical, is a fundamental component in digital logic. **Using only universal two-input NOR gates**, design and draw the logic circuit that produces the XNOR function: **F = AB + A'B'**. [Marks-3]

**b)** Analyze the complex logic circuit shown below:
    1.  Carefully derive the final Boolean expression for the output F.
    2.  Simplify this expression to its most minimal form by applying the laws of Boolean algebra. You may need to use advanced theorems like the Consensus theorem.
    3.  Create a full truth table to prove that your simplified expression is logically identical to the original complex expression. [Marks-7]

```
                         +----[ AND G1 ]----+
       +--------|>o------|                 |
       |                 |                 |
A -----+-----------------|----[ AND G2 ]----|----[ OR G3 ]---- F
       |                 |                 |
       |                 +----[ AND G3 ]    |
B -----+-----------------|                 |
                         |                 |
C -----------------------+----[ AND G3 ]

```
*(Diagram: A feeds G2. B feeds G1 and G3. A goes into a NOT gate whose output A' feeds G1. C feeds G3. The outputs of G1, G2, and G3 all feed into the final OR gate.)*

---

### **Solutions and Detailed Explanations**

#### **Question 1(a): Evolving Role of the CU and ALU**

**Answer:**
This question compares the processor components of a **Second Generation** computer with a **Fifth Generation** computer.

**Analysis of the Evolving Roles:**

*   **Arithmetic Logic Unit (ALU):** The fundamental role of the ALU has remained the most consistent.
    *   **2nd Gen:** The ALU performed arithmetic (add, subtract) and logical (AND, OR) operations on data fed to it by the CU. It was a simple, powerful calculator.
    *   **5th Gen:** The modern ALU is vastly more complex, handling floating-point math, vector operations, and complex logical comparisons. However, its core function is the same: **it is the computational engine**. In both eras, it executes the operations; it does not decide *what* to execute next.

*   **Control Unit (CU):** The role of the CU has changed dramatically, evolving from a simple sequencer to a sophisticated manager.
    *   **2nd Gen (Batch Model):** The CU was a **rigid instruction follower**. It would fetch an instruction from magnetic tape, decode it, and execute it, then fetch the next one in a strict, linear sequence. Its primary job was to execute a single, long-running program without interruption. There was no concept of multitasking or context switching.
    *   **5th Gen (Multitasking Model):** The CU is a **dynamic operation manager**. It still fetches-decodes-executes, but it does so under the direction of the Operating System. Its key new roles include:
        *   **Context Switching:** Rapidly switching between different programs (contexts), saving the state of one to run another.
        *   **Pipeline and Branch Prediction:** It sophisticatedly manages instruction pipelines to execute multiple stages of different instructions at once and predicts future program paths to pre-load data.
        *   **Interrupt Handling:** It must constantly handle interrupts from I/O devices, timers, and the OS, pausing the current task to serve a higher-priority one.

**Philosophical Shift:** The CPU's role changed from being a **monolithic calculator** for a single task to a **high-speed, manageable resource** that can be shared among dozens of concurrent tasks, creating the illusion of parallel execution for the user. The CU evolved from a "foreman" on an assembly line to an "air traffic controller" managing many planes at once.

---

#### **Question 1(b): Memory Comparison (Registers vs. L1 Cache)**

**Answer:**
*   **Memory A (Current Instruction):** These are **CPU Registers**.
*   **Memory B (Next Likely Instructions):** This is **L1 Cache**.

**Comparison:**

| Feature | CPU Registers | L1 Cache |
| :--- | :--- | :--- |
| **Precise Function** | Holds the **immediate data** (operands, addresses, instruction pointers) that the ALU is **currently processing** in a given clock cycle. They are the ALU's direct workspace. | Holds a **small copy of data and instructions from RAM** that the CPU predicts it will need very soon. It acts as a buffer to prevent waiting for slower RAM. |
| **Position & Speed**| **Top of the memory hierarchy.** Physically part of the ALU and CU. **Fastest possible access** (effectively zero-latency for the ALU). | **Second in the hierarchy.** Sits right next to the core. **Extremely fast**, but with a few clock cycles of latency. Slower than registers. |
| **Size & Capacity**| **Extremely small.** Measured in bytes (e.g., 32 or 64 general-purpose registers, each 64-bits wide). | **Very small, but larger than registers.** Measured in kilobytes (e.g., 32KB, 64KB per core). |
| **Necessity** | **Absolutely essential.** The CPU cannot perform any operation without registers to hold the operands and results. | **Essential for modern performance.** A CPU without cache would be drastically slowed down, constantly waiting for RAM (the "von Neumann bottleneck"). Both are needed to create a smooth flow of data to the ALU. |

---

#### **Question 1(c): Number System Conversions**

**i) Convert 421₅ to Base 15**
*   **Step 1: Convert to Base 10.**
    *   421₅ = (4×5²) + (2×5¹) + (1×5⁰) = (4×25) + 10 + 1 = 100 + 10 + 1 = **111₁₀**.
*   **Step 2: Convert to Base 15.**
    *   111 ÷ 15 = 7 R 6.
    *   7 ÷ 15 = 0 R 7.
*   **Final Answer: 76₁₅**

**ii) Convert 11010.011₂ to Base 4**
*   Since 4 = 2², group binary digits in pairs.
*   **Integer Part:** From right `01 10 10`. (Pad with a zero).
    *   `01₂ = 1₄`, `10₂ = 2₄`, `10₂ = 2₄`. Result: `122₄`.
*   **Fractional Part:** From left `01 10`. (Pad with a zero).
    *   `01₂ = 1₄`, `10₂ = 2₄`. Result: `.12₄`.
*   **Final Answer: 122.12₄**

**iii) Convert 213.875₁₀ to Base 2**
*   **Integer Part (213):**
    *   213 ÷ 2 = 106 R 1
    *   106 ÷ 2 = 53 R 0
    *   53 ÷ 2 = 26 R 1
    *   26 ÷ 2 = 13 R 0
    *   13 ÷ 2 = 6 R 1
    *   6 ÷ 2 = 3 R 0
    *   3 ÷ 2 = 1 R 1
    *   1 ÷ 2 = 0 R 1. Result: **11010101₂**.
*   **Fractional Part (0.875):**
    *   0.875 × 2 = **1**.75
    *   0.75 × 2 = **1**.5
    *   0.5 × 2 = **1**.0. Result: **.111₂**.
*   **Final Answer: 11010101.111₂**

---

#### **Question 2(a): XNOR Gate from NOR Gates**
The expression for XNOR is F = AB + A'B'. This requires a 5-gate NOR implementation.
```
         +----[ NOR G4 ]----+
A --+----|                 |
  |    |                 |----[ NOR G5 ]---- F = A XNOR B
  +----|----[ NOR G1 ]----+
       |
       |----[ NOR G2 ]----+
B --+----|                 |
  |    +----[ NOR G3 ]----+
  +------------------------+
```

---

#### **Question 2(b): Analyze and Simplify Logic Circuit**

**1. Identify Final Output Expression:**
*   **G1 (AND Gate):** Inputs are A' and B. Output = `A'B`.
*   **G2 (AND Gate):** Input is A. Output = `A`. (Since it's a 1-input AND, it's just a buffer).
*   **G3 (AND Gate):** Inputs are B and C. Output = `BC`.
*   **Final OR Gate** combines the outputs of G1, G2, and G3.
*   **Final Expression: F = A'B + A + BC**

**2. Simplify the Expression:**
*   `F = A + A'B + BC`
*   First, rearrange using the Commutative Law: `F = (A + A'B) + BC`
*   Apply the **Redundancy Law** (`X + X'Y = X + Y`) to the parentheses.
    *   `A + A'B` simplifies to `A + B`.
*   The expression is now: `F = (A + B) + BC`
*   Rearrange again: `F = A + (B + BC)`
*   Apply the **Absorption Law** (`X + XY = X`) to the new parentheses.
    *   `B + BC` simplifies to `B`.
*   **Simplified Expression: F = A + B**

    *Self-Correction: The question asked for Consensus Theorem. Let's re-simplify using that view.*
    *   Initial: `F = AB + A'C + BC`
    *   **Consensus Theorem:** `XY + X'Z + YZ = XY + X'Z`. The `YZ` term is redundant.
    *   In our expression `F = A + A'B + BC`:
        *   This does not match the Consensus form directly. The absorption/redundancy law method is more direct here. Let's use it as it's simpler and more applicable. The final simplified form is indeed A+B.

**3. Prove with a Truth Table:**

| **A** | **B** | **C** | **Original F** (A + A'B + BC) | **Simplified F (A+B)** |
|:---:|:---:|:---:|:---:|:---:|
| 0 | 0 | 0 | 0 | **0** | **0** |
| 0 | 0 | 1 | 0 | **0** | **0** |
| 0 | 1 | 0 | 1 | **1** | **1** |
| 0 | 1 | 1 | 1 | **1** | **1** |
| 1 | 0 | 0 | 1 | **1** | **1** |
| 1 | 0 | 1 | 1 | **1** | **1** |
| 1 | 1 | 0 | 1 | **1** | **1** |
| 1 | 1 | 1 | 1 | **1** | **1** |

**Conclusion:**
The output columns for the original complex expression and the simplified expression are identical, proving that the circuit logically simplifies to F = A + B. The `BC` term was redundant.

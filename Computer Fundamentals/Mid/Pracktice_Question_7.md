### **Practice Midterm Question 07**

**Daffodil International University**
**Department of Software Engineering**
**Midterm Examination, Spring 2025**
**Course Code: SE 111; Course Title: Computer Fundamentals**

**Time: 1 Hour 30 Mins**
**Marks: 25**

**Answer ALL Questions**
---

**1. a)** You are presented with two computer systems from different eras:
    *   **System X (from 1970):** A minicomputer built with Integrated Circuits, running a timesharing OS that allows multiple programmers to work simultaneously.
    *   **System Y (from 1985):** A desktop personal computer with a microprocessor, running a graphical user interface (GUI) and connected to a local printer.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Identify the generation of each system and compare the key technological shifts in both hardware and software between these two eras.** [Marks-3]

**b)** A modern computer performs two critical tasks. First, when it boots up, it reads instructions from a non-volatile chip that tells it how to initialize hardware. Later, when running a high-performance game, the CPU frequently fetches graphics data from a small, exceptionally fast memory unit located directly on the processor to avoid lag. [Marks-3]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Identify the two types of memory being used (one for booting, one for high-performance gaming). Compare them based on their purpose, speed, and typical location.**

**c)** Perform the following number system conversions, showing your work clearly: [Marks-9]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; i) Convert **512₆** to its equivalent number in Base 12. (Remember: In Base 12, A=10, B=11).
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ii) Convert **17.4₈** to its Base 10 (Decimal) equivalent.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; iii) Convert **10110111.011₂** to its Base 16 (Hexadecimal) equivalent.

---

**2. a)** Illustrate a logic circuit that correctly represents the structure and operator precedence of the following Boolean expression: [Marks-3]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**F = A(B + C')' + B'C**

**b)** Analyze the logic circuit provided below:
    1.  Determine the final Boolean expression for the output F.
    2.  Simplify this expression to its most minimal form using the laws of Boolean algebra.
    3.  Create a complete truth table to verify that your simplified expression is logically equivalent to the original one from the circuit. [Marks-7]

```
                         +----[ AND G1 ]----+
       +--------|>o------|                 |
       |                 |                 |----[ OR G3 ]---- F (Output)
A -----+-----------------+-----------------|
       |
       |                 +----[ AND G2 ]----+
B -----|-----------------|
       |                 |
C -----+-----------------+----[ AND G2 ]

```
*(Diagram: A feeds G3 directly and also a NOT gate. B feeds G1 and G2. The output of the NOT gate (A') feeds G1. C feeds G2. The outputs of G1 and G2 feed G3.)*

---

### **Solutions and Detailed Explanations**

#### **Question 1(a): Comparison of Computer Generations**

**Answer:**
*   **System X** belongs to the **Third Generation (1964-1975)**.
*   **System Y** belongs to the **Fourth Generation (1975-1989)**.

**Comparison of Technological Shifts:**

| Feature | Third Generation (System X) | Fourth Generation (System Y) | **Key Shift (পরিবর্তন)** |
| :--- | :--- | :--- | :--- |
| **Core Hardware** | **Integrated Circuits (ICs)** containing dozens of transistors. | **Microprocessors** built with **VLSI (Very Large-Scale Integration)** containing thousands or millions of transistors. | **Miniaturization and Integration.** The entire CPU moved from multiple ICs onto a single chip, leading to the Personal Computer. |
| **Computer Type** | **Minicomputers** shared by many users. | **Personal Computers (PCs)** for individual users. | A move from **shared, centralized computing** to **distributed, individual computing**. |
| **Software Interface**| **Command-Line Interface** on terminals (Text-based). | **Graphical User Interface (GUI)** with icons and a mouse (Visual). | **Improved Usability.** The shift made computers accessible to the general public, not just experts. |
| **Primary Use** | Scientific and business applications in organizations. | Productivity (word processing, spreadsheets), education, and entertainment for individuals. | Computing became a **personal tool** rather than just an organizational one. |

---

#### **Question 1(b): Memory Comparison (ROM vs. Cache)**

**Answer:**
*   The memory for booting is **ROM (Read-Only Memory)**.
*   The high-performance gaming memory is **Cache Memory**.

**Comparison:**

| Feature | ROM (for Booting) | Cache Memory (for Gaming Performance) |
| :--- | :--- | :--- |
| **Purpose (উদ্দেশ্য)**| To permanently store firmware (like BIOS) that is essential for starting the computer. (কম্পিউটার চালু করার জন্য স্থায়ী নির্দেশনা ধারণ করে)। | To temporarily store frequently accessed data and instructions to provide the CPU with high-speed access, preventing bottlenecks. (দ্রুত ডেটা সরবরাহের জন্য ব্যবহৃত হয়)। |
| **Speed (গতি)** | **Slow** in comparison to CPU and RAM. Its speed is not critical as it's only read at startup. (ধীরগতির)। | **Extremely Fast**. It is the fastest memory in a computer system, designed to match the CPU's speed. (অত্যন্ত দ্রুত)। |
| **Typical Location** | A dedicated chip on the **motherboard**. (মাদারবোর্ডে থাকা একটি চিপ)। | Integrated **directly onto the CPU die** (L1, L2 cache) or placed very close to it on the motherboard (L3 cache). (সিপিইউ-এর ভিতরে বা খুব কাছে থাকে)। |
| **Volatility (উদ্বায়ীতা)** | **Non-Volatile** (retains data without power). | **Volatile** (loses data without power). |

---

#### **Question 1(c): Number System Conversions**

**i) Convert 512₆ to Base 12**
*   **Step 1: Convert from Base 6 to Base 10.**
    *   512₆ = (5 × 6²) + (1 × 6¹) + (2 × 6⁰)
    *   = (5 × 36) + (1 × 6) + (2 × 1)
    *   = 180 + 6 + 2 = **188₁₀**
*   **Step 2: Convert from Base 10 to Base 12.**
    *   188 ÷ 12 = 15 R 8
    *   15 ÷ 12 = 1 R 3
    *   1 ÷ 12 = 0 R 1
    *   Read bottom-up: **138₁₂**
*   **Final Answer: 512₆ = 138₁₂**

**ii) Convert 17.4₈ to Base 10**
*   (1 × 8¹) + (7 × 8⁰) + (4 × 8⁻¹)
    = 8 + 7 + (4 / 8)
    = 15 + 0.5
    = **15.5₁₀**

**iii) Convert 10110111.011₂ to Base 16**
*   **Integer Part:** Group bits into sets of 4 from the right. `1011 0111`
*   **Fractional Part:** Group bits into sets of 4 from the left. `0110` (pad with a zero).
*   Convert each group:
    *   `1011₂` = 8+2+1 = 11₁₀ = **B₁₆**
    *   `0111₂` = 4+2+1 = 7₁₀ = **7₁₆**
    *   `0110₂` = 4+2 = 6₁₀ = **6₁₆**
*   **Final Answer: B7.6₁₆**

---

#### **Question 2(a): Illustrate Logic Circuit**

**Expression: F = A(B + C')' + B'C**
1.  **C'**: C goes into a NOT gate.
2.  **B + C'**: B and the output of the NOT gate (C') go into an OR gate.
3.  **(B + C')'**: The output of this OR gate goes into another NOT gate (forming a NOR).
4.  **A(B + C')'**: A and the output of the second NOT gate go into an AND gate.
5.  **B'C**: B is inverted with a NOT gate, then ANDed with C.
6.  **Final F**: The outputs from the two main AND gates (steps 4 and 5) are combined in a final OR gate.

---

#### **Question 2(b): Analyze and Simplify Logic Circuit**

**1. Identify Final Output Expression:**
*   **G1 (AND Gate):** Inputs are A' and B. Output = `A'B`.
*   **G2 (AND Gate):** Inputs are B and C. Output = `BC`.
*   **G3 (OR Gate):** Inputs are `A`, `A'B`, and `BC`.
*   **Final Expression: F = A + A'B + BC**

**2. Simplify the Expression:**
*   `F = A + A'B + BC`
*   First, apply the **Redundancy Law** to the first two terms: `X + X'Y = X + Y`.
    *   Here, X=A and Y=B. So, `A + A'B` simplifies to `A + B`.
*   The expression is now: `F = (A + B) + BC`
*   Now, apply the **Absorption Law** which states `X + XY = X`.
    *   Let X = B and Y = C in the sub-expression `B + BC`. This simplifies to just `B`.
    *   Let's regroup: `F = A + (B + BC)`.
    *   `F = A + B`
*   *Alternative simplification (Consensus Theorem):* The theorem `X Y + X'Z + Y Z = X Y + X'Z` states the YZ term is redundant. In our expression `A•1 + A'B + B•1`, it is a different form. Let's stick with the first method. The correct simplification for `A + B + BC` is `A+B` as `B+BC` simplifies to `B`.
*   **Simplified Expression: F = A + B**

**3. Prove with a Truth Table:**

| **A**| **B**| **C**| **A'**| **A'B**(G1) | **BC**(G2)| **Original F** (A+A'B+BC) | **Simplified F (A+B)**|
| :---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 0 | 0 | 0 | 1 | 0 | 0 | **0** | **0** |
| 0 | 0 | 1 | 1 | 0 | 0 | **0** | **0** |
| 0 | 1 | 0 | 1 | 1 | 0 | **1** | **1** |
| 0 | 1 | 1 | 1 | 1 | 1 | **1** | **1** |
| 1 | 0 | 0 | 0 | 0 | 0 | **1** | **1** |
| 1 | 0 | 1 | 0 | 0 | 0 | **1** | **1** |
| 1 | 1 | 0 | 0 | 0 | 0 | **1** | **1** |
| 1 | 1 | 1 | 0 | 0 | 1 | **1** | **1** |

**Conclusion:**
The output columns for the original expression (`A + A'B + BC`) and the simplified expression (`A + B`) are identical, confirming that the simplification is correct. The `BC` term was redundant.

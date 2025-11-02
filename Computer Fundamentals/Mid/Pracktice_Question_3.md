

### **Practice Midterm Question 03**

**Daffodil International University**
**Department of Software Engineering**
**Midterm Examination, Spring 2025**
**Course Code: SE 111; Course Title: Computer Fundamentals**

**Time: 1 Hour 30 Mins**
**Marks: 25**

**Answer ALL Questions**
---

**1. a)** A museum is restoring a computer from the 1960s. The machine is large, uses **transistors** instead of vacuum tubes, and was programmed using early high-level languages like **FORTRAN** for complex scientific calculations. Data was stored on **magnetic tapes**, and programs were run one by one in a batch. [Marks-3]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Based on this description, identify and explain the generation of this computer, including its core hardware and software technologies.**

**b)** A computer hardware engineer is designing a new high-performance motherboard. For the CPU cache, she requires extremely fast memory that holds data as long as power is supplied without needing to be refreshed. For the main memory, she chooses a denser, more cost-effective type that stores data in capacitors and requires a periodic refresh cycle to retain its information. [Marks-3]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Identify and compare these two distinct types of RAM.**

**c)** Perform the following number system conversions, showing all required calculations: [Marks-9]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; i) Convert **45.625₁₀** to its Base 2 (Binary) equivalent.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ii) Convert **B2F₁₆** to its Base 10 (Decimal) equivalent.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; iii) Convert **123₇** to its Base 9 equivalent.

---

**2. a)** Create a clear and labeled logic circuit diagram for the following Boolean expression: [Marks-3]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**F = (A • B + C)' + A' • B**

**b)** For the logic circuit provided below, perform the following tasks:
    1.  Derive the final Boolean expression for the output F.
    2.  Simplify the expression using the laws of Boolean algebra.
    3.  Prove that your simplification is correct by constructing a complete truth table. [Marks-7]

```
                +----[ OR  G1 ]----+
A --------------|                 |
                +----|>o----------|----[ AND G2 ]---- F (Output)
                                  |
B --------------------------------+
```
*(Note: `|>o` represents a NOT gate, `[OR Gx]` and `[AND Gx]` are logic gates.)*

---

### **Solutions and Detailed Explanations**

#### **Question 1(a): Computer Generation (2nd Generation)**

**Answer:**
The generation described is the **Second Generation of Computers (1955-1964)**.

**Explanation:**
The keywords "transistors," "FORTRAN," "magnetic tapes," and "batch processing" are the defining features of this era.

*   **Key Hardware:** The major breakthrough was the **Transistor**, which replaced the bulky and unreliable vacuum tubes of the first generation. This made computers significantly smaller, faster, cheaper, and more energy-efficient. Primary memory was made of **magnetic cores**, and **magnetic tapes and disks** were used for secondary storage.
*   **Key Software Technologies:**
    1.  **High-Level Programming Languages:** Early high-level languages like **FORTRAN** (for scientific and engineering problems) and **COBOL** (for business applications) were developed, making programming easier than writing in assembly or machine language.
    2.  **Batch Operating Systems:** These were early operating systems that allowed jobs (programs) to be collected in a "batch" and run sequentially without manual intervention between them, improving efficiency.

**Bengali Meaning (বাংলা অর্থ):**
*   **Transistor (ট্রানজিস্টর):** একটি অর্ধপরিবাহী যন্ত্র যা ভ্যাকুয়াম টিউবের পরিবর্তে ব্যবহৃত হতো।
*   **Magnetic Tape (ম্যাগনেটিক টেপ):** ডেটা সংরক্ষণের জন্য ব্যবহৃত চৌম্বকীয় ফিতা।
*   **Batch Operating System (ব্যাচ অপারেটিং সিস্টেম):** প্রোগ্রামগুলোকে একসাথে গ্রুপ করে পর্যায়ক্রমে চালানোর সিস্টেম।

**Easy Remember Trick (মনে রাখার কৌশল):**
Remember the **"T"** and **"B"** of the 2nd Gen:
*   **T**ransistors (The core hardware)
*   **B**atch Systems and **B**usiness/Science Languages (FORTRAN/COBOL)

---

#### **Question 1(b): Memory Comparison (SRAM vs. DRAM)**

**Answer:**
The two types of RAM are **SRAM (Static RAM)** and **DRAM (Dynamic RAM)**.

*   **SRAM** is used for the CPU cache because it is fast and does not need refreshing.
*   **DRAM** is used for the main memory because it is cheaper and has a higher density.

**Comparison:**

| Feature (বৈশিষ্ট্য) | SRAM (Static RAM) | DRAM (Dynamic RAM) |
| :--- | :--- | :--- |
| **Technology (প্রযুক্তি)** | Uses latches (flip-flops) to store each bit. | Uses a capacitor and a transistor to store each bit. |
| **Speed (গতি)** | **Faster.** Does not need to be refreshed. (অনেক দ্রুত)। | **Slower.** Must be periodically refreshed to maintain data. (ধীরগতির এবং রিফ্রেশ করা লাগে)। |
| **Size & Density (আকার)** | Less dense, meaning fewer memory cells per unit area. Physically larger for the same capacity. | Very dense, allowing for larger capacities in smaller physical spaces. |
| **Cost (খরচ)** | **More expensive** per bit. (দামে বেশি)। | **Cheaper** per bit. (দামে সস্তা)। |
| **Primary Use (ব্যবহার)** | **CPU Cache Memory**, high-speed registers. | **Main System Memory (RAM)**. |

**Easy Remember Trick (মনে রাখার কৌশল):**
*   **S**RAM is **S**uper-fast and **S**teady (no refresh).
*   **D**RAM is **D**ense and must be **D**ynamically refreshed.

---

#### **Question 1(c): Number System Conversions**

**i) Convert 45.625₁₀ to Base 2**
*   **Integer Part (45):** Use division-remainder.
    *   45 ÷ 2 = 22 R 1
    *   22 ÷ 2 = 11 R 0
    *   11 ÷ 2 = 5 R 1
    *   5 ÷ 2 = 2 R 1
    *   2 ÷ 2 = 1 R 0
    *   1 ÷ 2 = 0 R 1
    *   Integer part in binary (bottom-up): **101101₂**
*   **Fractional Part (0.625):** Use repeated multiplication by 2.
    *   0.625 × 2 = **1**.25
    *   0.25 × 2 = **0**.50
    *   0.50 × 2 = **1**.00
    *   Fractional part in binary (top-down): **.101₂**
*   **Combine:** **101101.101₂**

**ii) Convert B2F₁₆ to Base 10**
*   B2F₁₆ = (B × 16²) + (2 × 16¹) + (F × 16⁰)
    = (11 × 256) + (2 × 16) + (15 × 1)
    = 2816 + 32 + 15
    = **2863₁₀**

**iii) Convert 123₇ to Base 9**
*   **Step 1: Convert from Base 7 to Base 10.**
    *   123₇ = (1 × 7²) + (2 × 7¹) + (3 × 7⁰)
    *   = (1 × 49) + (2 × 7) + (3 × 1)
    *   = 49 + 14 + 3 = **66₁₀**
*   **Step 2: Convert from Base 10 to Base 9.**
    *   66 ÷ 9 = 7 R 3
    *   7 ÷ 9 = 0 R 7
    *   Read from bottom up: **73₉**
*   **Final Answer: 123₇ = 73₉**

---

#### **Question 2(a): Illustrate Logic Circuit**

**Expression: F = (A • B + C)' + A' • B**
1.  **A'**: Input A goes into a **NOT** gate.
2.  **A' • B**: The output from the NOT gate (A') and input B go into an **AND** gate.
3.  **A • B**: Inputs A and B go into another **AND** gate.
4.  **A • B + C**: The output of this AND gate and input C go into an **OR** gate.
5.  **(A • B + C)'**: The output of the OR gate goes into a **NOT** gate (this is a NOR operation).
6.  **Final F**: The outputs from step 2 and step 5 are combined in a final **OR** gate.

---

#### **Question 2(b): Analyze and Simplify Logic Circuit**

**1. Identify Final Output Expression:**
*   **G1 (OR Gate):** Inputs are A and B. Output = `A + B`
*   The `A` input also goes into a **NOT Gate**. Output = `A'`
*   **G2 (Final AND Gate):** Inputs are the output from G1 (`A + B`) and the output from the NOT Gate (`A'`).
*   **Final Expression: F = (A + B) • A'**

**2. Simplify the Expression:**
*   `F = (A + B)A'`
*   `F = A•A' + B•A'` *(Distributive Law)*
*   We know that `X•X' = 0` *(Complement Law)*. Therefore, `A•A' = 0`.
*   `F = 0 + BA'`
*   `F = BA'` or **A'B** *(Identity Law)*
*   **Simplified Expression: F = A'B**

**3. Prove with a Truth Table:**
We need to prove that `(A + B)A'` is identical to `A'B`. Since C is not an input, we only need a truth table for A and B.

| **A** | **B** | **A'** | **A + B** (G1) | **Original F** ( (A+B)A' ) | **Simplified F (A'B)** |
| :--- | :-: | :-: | :---: | :---: | :---: |
| 0 | 0 | 1 | 0 | **0** | **0** |
| 0 | 1 | 1 | 1 | **1** | **1** |
| 1 | 0 | 0 | 1 | **0** | **0** |
| 1 | 1 | 0 | 1 | **0** | **0** |

**Conclusion:**
Because the columns for **Original F** and **Simplified F** are identical for all combinations of inputs A and B, the simplification **F = A'B** is correct.

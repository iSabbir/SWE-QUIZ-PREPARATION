### **Practice Midterm Question 06**

**Daffodil International University**
**Department of Software Engineering**
**Midterm Examination, Spring 2025**
**Course Code: SE 111; Course Title: Computer Fundamentals**

**Time: 1 Hour 30 Mins**
**Marks: 25**

**Answer ALL Questions**
---

**1. a)** An office in the mid-1980s upgrades its typewriters to a fleet of the first commercially successful personal computers. These machines are powered by **microprocessors** using **Very Large-Scale Integration (VLSI)**. Employees use these standalone machines for word processing and spreadsheets, and the company is planning its first **Local Area Network (LAN)** to share a printer. [Marks-3]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Identify this computer generation. Describe its defining hardware and software features based on the scenario.**

**b)** A student has a 1 GB USB drive. She needs to store a term paper that is 1024 KB in size and a collection of photos, each averaging 4 MB. Explain the relationship between the memory units KB, MB, and GB. Calculate the maximum number of 4 MB photos she can store on the drive after saving her term paper. [Marks-3]

**c)** Perform the following number system conversions, clearly outlining each step of the process: [Marks-9]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; i) Convert **432₅** to its equivalent in Base 7.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ii) Convert **11011.11₂** to its Base 10 (Decimal) equivalent.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; iii) Convert **1F9.A₁₆** to its Base 2 (Binary) equivalent.

---

**2. a)** A key principle in Boolean algebra is Operator Precedence. For the expression **F = A + B • C'**, explain the order in which the operations (OR, AND, NOT) would be evaluated. Illustrate this expression with a logic circuit diagram that reflects this precedence. [Marks-3]

**b)** Analyze the logic circuit diagram provided below:
    1.  Derive the final Boolean expression for the output F.
    2.  Using the laws of Boolean algebra (specifically the Redundancy Rule), simplify the expression to its most minimal two-variable form.
    3.  Create a truth table to prove that your simplified expression is logically equivalent to the original expression derived from the circuit. [Marks-7]

```
                         +----[ AND G1 ]----+
       +--------|>o------|                 |
       |                 +-----------------|----[ OR G2 ]---- F (Output)
A -----+-----------------------------------+
       |
B -----+-----------------[ AND G1 ]

```
*(Diagram: Input A goes to OR gate G2 and NOT gate. Input B goes to AND gate G1. The output of the NOT gate (A') also goes to G1. The output of G1 goes to the OR gate G2.)*

---

### **Solutions and Detailed Explanations**

#### **Question 1(a): Computer Generation (4th Generation)**

**Answer:**
This scenario describes the **Fourth Generation of Computers (1975-1989)**.

**Explanation:**
The keywords **microprocessors**, **Very Large-Scale Integration (VLSI)**, **personal computers**, and **Local Area Networks (LAN)** are hallmarks of this era.

*   **Key Hardware:**
    *   **Microprocessor & VLSI:** The central innovation was the microprocessor, a complete CPU on a single chip. This was made possible by VLSI technology, which allowed hundreds of thousands (and later, millions) of components on one chip.
    *   **Personal Computers (PCs):** The microprocessor made computers small, cheap, and powerful enough for individuals and small businesses to own, leading to the PC revolution.
*   **Key Software Technologies:**
    *   **Graphical User Interfaces (GUIs):** GUIs, mice, and user-friendly operating systems (like MS-DOS and early versions of Windows and Mac OS) made computers accessible to non-technical users.
    *   **Application Software:** The rise of PCs created a huge market for software like word processors (WordStar), spreadsheets (VisiCalc, Lotus 1-2-3), and databases.
    *   **Computer Networking:** The development of **Local Area Networks (LANs)** allowed PCs to connect to share resources like printers and files, laying the groundwork for the internet.

**Bengali Meaning (বাংলা অর্থ):**
*   **VLSI (Very Large-Scale Integration):** একটি একক চিপে লক্ষাধিক উপাদান স্থাপন করার প্রযুক্তি।
*   **Personal Computer (PC):** ব্যক্তিগত ব্যবহারের কম্পিউটার।
*   **Local Area Network (LAN):** সীমিত এলাকা জুড়ে কম্পিউটার নেটওয়ার্ক।

**Easy Remember Trick (মনে রাখার কৌশল):**
4th Gen brought computing from the **Lab to your Lap**:
*   **M**icroprocessor, **N**etworks, and **G**UIs made computers **P**ersonal.

---

#### **Question 1(b): Memory Units and Calculation**

**Answer:**
**Relationship between Units:**
Computer memory is measured in bytes. The prefixes Kilo (K), Mega (M), and Giga (G) represent powers of 2.
*   **1 Kilobyte (KB)** = 1024 Bytes
*   **1 Megabyte (MB)** = 1024 Kilobytes (KB)
*   **1 Gigabyte (GB)** = 1024 Megabytes (MB)
Each unit is 1024 times larger than the previous one.

**Calculation:**
1.  **Total Drive Space in MB:**
    *   1 GB = 1024 MB

2.  **Convert Paper Size to MB:**
    *   The paper is 1024 KB. Since 1 MB = 1024 KB, the paper size is exactly **1 MB**.

3.  **Calculate Remaining Space:**
    *   Remaining Space = Total Space - Paper Space
    *   Remaining Space = 1024 MB - 1 MB = **1023 MB**

4.  **Calculate Number of Photos:**
    *   Number of Photos = Remaining Space / Size per Photo
    *   Number of Photos = 1023 MB / 4 MB = **255.75**

Since she cannot store a fraction of a photo, the maximum number of photos she can store is **255**.

---

#### **Question 1(c): Number System Conversions**

**i) Convert 432₅ to Base 7**
*   **Step 1: Convert from Base 5 to Base 10.**
    *   432₅ = (4 × 5²) + (3 × 5¹) + (2 × 5⁰)
    *   = (4 × 25) + (3 × 5) + (2 × 1)
    *   = 100 + 15 + 2 = **117₁₀**
*   **Step 2: Convert from Base 10 to Base 7.**
    *   117 ÷ 7 = 16 R 5
    *   16 ÷ 7 = 2 R 2
    *   2 ÷ 7 = 0 R 2
    *   Read bottom-up: **225₇**
*   **Final Answer: 432₅ = 225₇**

**ii) Convert 11011.11₂ to Base 10**
*   **Integer Part (11011):**
    *   (1×2⁴) + (1×2³) + (0×2²) + (1×2¹) + (1×2⁰)
    *   = 16 + 8 + 0 + 2 + 1 = **27**
*   **Fractional Part (.11):**
    *   (1×2⁻¹) + (1×2⁻²) = 0.5 + 0.25 = **0.75**
*   **Combine:** **27.75₁₀**

**iii) Convert 1F9.A₁₆ to Base 2**
*   Convert each Hex digit to its 4-bit binary representation.
    *   1₁₆ = 0001₂
    *   F₁₆ (15) = 1111₂
    *   9₁₆ = 1001₂
    *   A₁₆ (10) = 1010₂
*   **Final Answer: 000111111001.1010₂** (Leading zeros can be omitted: `111111001.101` )

---

#### **Question 2(a): Operator Precedence and Circuit Diagram**

**Expression: F = A + B • C'**
**Explanation of Precedence:**
In Boolean algebra, the order of operations is similar to standard math:
1.  **Parentheses/Brackets** (highest precedence, none in this expression).
2.  **NOT (')**: This operation is performed first. `C'` will be evaluated.
3.  **AND (•)**: This operation is performed next. The result of `C'` will be ANDed with `B`.
4.  **OR (+)**: This operation is performed last. `A` will be ORed with the result of `(B • C')`.

**Logic Circuit Diagram:**
The circuit must be drawn to reflect this order.
1.  Input C passes through a **NOT** gate.
2.  The output of the NOT gate (`C'`) and input B are connected to an **AND** gate.
3.  The output of the AND gate (`B • C'`) and input A are connected to a final **OR** gate, which produces F.

---

#### **Question 2(b): Analyze and Simplify Logic Circuit**

**1. Identify Final Output Expression:**
*   Input A is inverted, producing `A'`.
*   **G1 (AND Gate):** The inputs are `A'` and `B`. The output is `A'B`.
*   **G2 (OR Gate):** The inputs are the original input `A` and the output from G1 (`A'B`).
*   **Final Expression: F = A + A'B**

**2. Simplify the Expression:**
*   This expression uses the **Redundancy Law** (also called Adjacency or Absorption variation).
*   **Rule:** `X + X'Y = X + Y`
*   Applying this rule to our expression, where X = A and Y = B:
    *   `F = A + A'B`
    *   `F = A + B`
*   *Proof of the rule:*
    `A + A'B = (A + A')(A + B)`  *(Distributive Law)*
    `= 1 • (A + B)`        *(Complement Law: A+A'=1)*
    `= A + B`                *(Identity Law)*
*   **Simplified Expression: F = A + B**

**3. Prove with a Truth Table:**

| **A** | **B** | **A'** | **A'B** (G1) | **Original F** ( A + A'B ) | **Simplified F (A+B)** |
| :--- | :-: | :-: | :---: | :---: | :---: |
| 0 | 0 | 1 | 0 | **0** | **0** |
| 0 | 1 | 1 | 1 | **1** | **1** |
| 1 | 0 | 0 | 0 | **1** | **1** |
| 1 | 1 | 0 | 0 | **1** | **1** |

**Conclusion:**
The final output columns for the original circuit expression and the simplified expression are identical. This verifies that the logic `A + A'B` simplifies to `A + B`.

### **Practice Midterm Question 02**

**Daffodil International University**
**Department of Software Engineering**
**Midterm Examination, Spring 2025**
**Course Code: SE 111; Course Title: Computer Fundamentals**

**Time: 1 Hour 30 Mins**
**Marks: 25**

**Answer ALL Questions**
---

**1. a)** Alpha Innovations, a startup, has provided its employees with their first "Personal Computers" (PCs). These machines are compact enough to fit on a desk and are equipped with a microprocessor, a mouse, and a graphical user interface (GUI) operating system. This move has significantly increased productivity. [Marks-3]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Based on this scenario, identify and explain the computer generation, including its key hardware and software technologies.**

**b)** A computer's startup process involves reading initial instructions from a type of memory that cannot be altered and retains data even when powered off. Once the operating system is loaded, the computer uses a different, much faster type of memory to run applications, which loses its data when the computer is shut down. [Marks-3]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Compare the two types of memory mentioned in this scenario.**

**c)** Perform the following number system conversions: [Marks-9]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; i) Convert **275.4₈** to its Base 10 (Decimal) equivalent.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ii) Convert **423₁₀** to its Base 16 (Hexadecimal) equivalent.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; iii) Convert **562₈** to its Base 16 (Hexadecimal) equivalent.

---

**2. a)** Illustrate a logic circuit for the following Boolean expression: [Marks-3]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**F = (A+B)' • C + A • (B+C')**

**b)** For the logic circuit diagram shown below, identify the final output expression. Then, simplify the expression using Boolean algebra rules and prove your simplification is correct using a truth table. [Marks-7]

```
A ---|>o-----+----[AND G1]--+
             |              |
B -----------+----[AND G1]--+----[OR]---- F (Output)
   |         |              |
   +---------+----[AND G2]--+
             |
C ---|>o-----+----[AND G2]
```
*(Here, `|>o--` represents a NOT gate, `[AND Gx]` represents an AND gate, and `[OR]` is an OR gate)*

---

### **Answers and Detailed Explanations**

#### **Question 1(a): Computer Generation**

**Answer:**
The generation described is the **Fourth Generation of Computers (1975-1989)**.

**Explanation:**
The key clues in the scenario are "Personal Computers (PCs)," "microprocessor," "mouse," and "graphical user interface (GUI)."

*   **Key Hardware:** The defining invention of this generation was the **microprocessor**. This single chip contained the entire Central Processing Unit (CPU), which made it possible to create small, affordable computers that could fit on a desk—the Personal Computer (PC).
*   **Key Software Technologies:**
    1.  **Graphical User Interfaces (GUIs):** Instead of command-line interfaces (like in the 3rd Gen), operating systems like MS-Windows and Apple Macintosh started using GUIs. This allowed users to interact with the computer using icons, windows, and a **mouse**, making them much more user-friendly.
    2.  **Spread of High-Level Languages:** Languages like C++ and Object-Oriented Programming concepts emerged and gained popularity.
    3.  **Computer Networks:** The development of Local Area Networks (LAN) and the beginnings of the modern internet took place during this time.

**Bengali Meaning (বাংলা অর্থ):**
*   **Microprocessor (মাইক্রোপ্রসেসর):** একটি একক চিপ যাতে সম্পূর্ণ CPU থাকে।
*   **Personal Computer (PC) (পার্সোনাল কম্পিউটার):** ব্যক্তিগত ব্যবহারের জন্য নির্মিত কম্পিউটার।
*   **GUI (Graphical User Interface):** ಚಿತ್ರভিত্তিক ইউজার ইন্টারফেস, যা আইকন ও মাউস দিয়ে কাজ করতে সাহায্য করে।

**Easy Remember Trick (মনে রাখার কৌশল):**
Fourth generation is all about the **"Micro-P"**:
*   **Micro**processor
*   **P**ersonal Computer (PC)

---

#### **Question 1(b): Memory Comparison (RAM vs. ROM)**

**Answer:**
The two types of memory are **ROM (Read-Only Memory)** and **RAM (Random Access Memory)**.

*   The memory for the startup process (BIOS) is **ROM**.
*   The memory for running active applications is **RAM**.

**Comparison:**

| Feature (বৈশিষ্ট্য) | ROM (Read-Only Memory) | RAM (Random Access Memory) |
| :--- | :--- | :--- |
| **Purpose (উদ্দেশ্য)** | Stores firmware like the BIOS to boot up the computer. (কম্পিউটার চালু করার প্রোগ্রাম ধারণ করে)। | Stores data and applications that are currently in use. (চলমান প্রোগ্রাম ও ডেটা ধারণ করে)। |
| **Volatility (উদ্বায়ীতা)** | **Non-Volatile**. Data is permanent and is not lost when power is off. | **Volatile**. Data is temporary and is lost when power is off. |
| **Operation (কার্যক্রম)** | Data can only be **read** from it. It cannot be easily modified. (শুধুমাত্র পড়া যায়, পরিবর্তন করা যায় না)। | Data can be **read and written**. It's the computer's workspace. (পড়া ও লেখা দুটোই যায়)। |
| **Example Use (উদাহরণ)** | Storing the computer's Basic Input/Output System (BIOS). | Loading a web browser or a game into memory. |

**Easy Remember Trick (মনে রাখার কৌশল):**
*   **RO**M is **R**ead-**O**nly and **R**emembers **O**ffline (permanent).
*   **RA**M is **R**andom **A**ccess and **R**uns **A**pps (temporary workspace).

---

#### **Question 1(c): Number System Conversions**

**i) Convert 275.4₈ to Base 10**
*   275.4₈ = (2 × 8²) + (7 × 8¹) + (5 × 8⁰) + (4 × 8⁻¹)
    = (2 × 64) + (7 × 8) + (5 × 1) + (4 × 1/8)
    = 128 + 56 + 5 + 0.5
    = **189.5₁₀**

**ii) Convert 423₁₀ to Base 16**
*   Use the division-remainder method. In hexadecimal, remainders 10-15 are represented by A-F.

| Division | Quotient | Remainder | Hex Value |
| :--- | :--- | :--- | :---: |
| 423 ÷ 16 | 26 | 7 | 7 |
| 26 ÷ 16 | 1 | 10 | A |
| 1 ÷ 16 | 0 | 1 | 1 |

*   Read from bottom to top: **1A7₁₆**

**iii) Convert 562₈ to Base 16**
*   Use binary as an intermediate step (shortcut).
*   **Step 1 (Octal to 3-bit Binary):**
    *   5₈ = 101₂
    *   6₈ = 110₂
    *   2₈ = 010₂
    *   Combined Binary: **101 110 010**
*   **Step 2 (Regroup into 4-bit Binary from right to left):**
    *   Add leading zeros if needed: **0001 0111 0010**
*   **Step 3 (4-bit Binary to Hex):**
    *   0001₂ = **1**₁₆
    *   0111₂ = **7**₁₆
    *   0010₂ = **2**₁₆
    *   **Final Answer: 172₁₆**

---

#### **Question 2(a): Illustrate Logic Circuit**

**Expression: F = (A+B)' • C + A • (B+C')**
The circuit would be drawn as:
1.  An **OR** gate for A and B.
2.  The output of the OR gate goes into a **NOT** gate (this is a NOR operation).
3.  The output of the NOT gate and input C go into an **AND** gate.
4.  A **NOT** gate for input C.
5.  Input B and the output of C's NOT gate go into an **AND** gate.
6.  The output of that AND gate and input A go into another **AND** gate.
7.  The outputs of the two main AND gates (from steps 3 and 6) go into a final **OR** gate to produce F.

---

#### **Question 2(b): Analyze and Simplify Logic Circuit**

**1. Identify Final Output Expression:**
*   **G1 (AND Gate):** Inputs are A' and B. Output = `A'B`
*   **G2 (AND Gate):** Inputs are B and C'. Output = `BC'`
*   The expression is incorrectly derived, G2 takes input A',B and C'. Output `A'BC'`
*   **Final OR Gate:** Inputs are outputs of G1 and G2.
*   **Final Expression: F = A'B + A'BC'**

**2. Simplify the Expression:**
*   `F = A'B + A'BC'`
*   `F = A'B (1 + C')`  *(Take A'B as common - Distributive Law)*
*   Since `1 + X = 1` in Boolean algebra (Annulment Law), `1 + C' = 1`.
*   `F = A'B • 1`
*   **Simplified Expression: F = A'B**

**3. Prove with a Truth Table:**
We will show that the column for the original expression (`A'B + A'BC'`) is identical to the simplified one (`A'B`).

| **A** | **B** | **C** | **A'** | **C'** | **A'B** (G1) | **A'BC'** (G2) | **Original F** (G1+G2) | **Simplified F (A'B)** |
| :--- | :-: | :-: | :-: | :-: | :---: | :---: | :---: | :---: |
| 0 | 0 | 0 | 1 | 1 | 0 | 0 | **0** | **0** |
| 0 | 0 | 1 | 1 | 0 | 0 | 0 | **0** | **0** |
| 0 | 1 | 0 | 1 | 1 | 1 | 1 | **1** | **1** |
| 0 | 1 | 1 | 1 | 0 | 1 | 0 | **1** | **1** |
| 1 | 0 | 0 | 0 | 1 | 0 | 0 | **0** | **0** |
| 1 | 0 | 1 | 0 | 0 | 0 | 0 | **0** | **0** |
| 1 | 1 | 0 | 0 | 1 | 0 | 0 | **0** | **0** |
| 1 | 1 | 1 | 0 | 0 | 0 | 0 | **0** | **0** |

**Conclusion:**
The columns for the **Original F** and the **Simplified F** are identical. Therefore, the simplification **F = A'B** is correct.

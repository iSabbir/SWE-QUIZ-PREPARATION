

### **Practice Midterm Question 04**

**Daffodil International University**
**Department of Software Engineering**
**Midterm Examination, Spring 2025**
**Course Code: SE 111; Course Title: Computer Fundamentals**

**Time: 1 Hour 30 Mins**
**Marks: 25**

**Answer ALL Questions**
---

**1. a)** A historical documentary shows computer scientists in the 1950s working with a machine that fills an entire room. This computer used thousands of **vacuum tubes**, generated immense heat, and frequently malfunctioned. Programmers fed it instructions using **punched cards**, and it could only process one program at a time, taking hours for a single calculation. [Marks-3]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Identify the computer generation being depicted. Explain its key hardware characteristics and software technologies.**

**b)** A data analyst needs to retrieve a file from a long-term archival system that uses **magnetic tapes**. To access the 500th record, the system must read through the first 499 records. In contrast, when she accesses a file on her laptop's **Solid State Drive (SSD)**, she can jump directly to the data's location almost instantly. [Marks-3]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Identify and compare the two different memory *access modes* demonstrated in this scenario.**

**c)** Execute the following number system conversions, ensuring you show the methodology for each: [Marks-9]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; i) Convert **C4E.8₁₆** to its Base 2 (Binary) equivalent.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ii) Convert **312₄** to its Base 8 (Octal) equivalent.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; iii) Convert **99₁₀** to its Base 2 (Binary) equivalent.

---

**2. a)** The NAND gate is a "universal gate" because any other logic gate can be constructed from it. **Using ONLY two-input NAND gates**, draw a logic circuit that replicates the function of a standard two-input OR gate (F = A + B). [Marks-3]

**b)** For the logic circuit illustrated below, complete the following:
    1.  Determine the final Boolean expression for the output F.
    2.  Simplify this expression to its most basic form using Boolean algebra laws (like De Morgan's theorem).
    3.  Validate your simplification by creating a truth table that compares the original expression to the simplified one. [Marks-7]

```
           +----|>o---+
A ---------|          |
           |          |----[ AND G1 ]----|>o---- F (Output)
           |          |
B ---------|          |
           +----|>o---+
```
*(Diagram represents: Inputs A and B each go into a NOT gate. The outputs of both NOT gates go into an AND gate. The output of the AND gate goes into a final NOT gate.)*

---

### **Solutions and Detailed Explanations**

#### **Question 1(a): Computer Generation (1st Generation)**

**Answer:**
This is the **First Generation of Computers (1942-1955)**.

**Explanation:**
The description of a room-sized machine using **vacuum tubes** and **punched cards** is the classic image of a first-generation computer.

*   **Key Hardware:**
    *   **Vacuum Tubes:** These were used as the primary electronic components for circuitry and memory. They were large, produced a lot of heat, were unreliable, and consumed a great deal of power.
    *   **Punched Cards and Paper Tape:** These were the primary methods for inputting data and programs and for storing output. Magnetic tape was introduced near the end of this era.
*   **Key Software Technologies:**
    *   **Machine Language:** Computers were programmed directly in binary (0s and 1s), which was incredibly difficult and machine-specific.
    *   **No Operating System:** There were no operating systems. Programmers had to interact with the raw hardware directly to execute a single program.
    *   **Example Systems:** ENIAC, EDVAC, UNIVAC I.

**Bengali Meaning (বাংলা অর্থ):**
*   **Vacuum Tube (ভ্যাকুয়াম টিউব):** প্রথম প্রজন্মের কম্পিউটারে ব্যবহৃত প্রধান ইলেকট্রনিক যন্ত্র।
*   **Punched Card (পাঞ্চড কার্ড):** ডেটা ইনপুট করার জন্য ব্যবহৃত ছিদ্রযুক্ত কার্ড।
*   **Machine Language (মেশিন ল্যাঙ্গুয়েজ):** শুধুমাত্র ০ এবং ১ ব্যবহার করে লেখা কম্পিউটারের মৌলিক ভাষা।

**Easy Remember Trick (মনে রাখার কৌশল):**
Think **"V"** for 1st Gen: **V**ery big, **V**ery hot, using **V**acuum tubes.

---

#### **Question 1(b): Memory Access Modes**

**Answer:**
The two access modes are **Sequential Access** (for the magnetic tape) and **Direct/Random Access** (for the SSD).

**Comparison:**

| Feature (বৈশিষ্ট্য) | Sequential Access (ধারাবাহিক অ্যাক্সেস) | Direct/Random Access (সরাসরি অ্যাক্সেস) |
| :--- | :--- | :--- |
| **Method (পদ্ধতি)** | Data is accessed in a specific, linear sequence. To get to a point, you must pass through everything before it. (ডেটা ক্রমানুসারে অ্যাক্সেস করা হয়)। | Any piece of data can be accessed directly by its address, regardless of its physical location. (যেকোনো ডেটা তার ঠিকানা দিয়ে সরাসরি অ্যাক্সেস করা যায়)। |
| **Speed (গতি)** | **Slow**, especially for data located far from the starting point. (ধীর)। | **Very fast** and access time is constant for any data location. (অনেক দ্রুত)। |
| **Typical Media** | **Magnetic Tape** is the classic example. | **RAM, SSD, Hard Disk Drives, CD/DVDs.** |
| **Analogy (উদাহরণ)** | Like a cassette tape: you must fast-forward to get to the middle of a song. | Like a music CD or MP3 file: you can instantly jump to any track. |

---

#### **Question 1(c): Number System Conversions**

**i) Convert C4E.8₁₆ to Base 2**
*   Convert each hexadecimal digit to its 4-bit binary equivalent.
    *   C₁₆ (12₁₀) = **1100₂**
    *   4₁₆ = **0100₂**
    *   E₁₆ (14₁₀) = **1110₂**
    *   (Decimal point)
    *   8₁₆ = **1000₂**
*   Combine them: **110001001110.1000₂**

**ii) Convert 312₄ to Base 8**
*   **Step 1: Convert from Base 4 to Base 10.**
    *   312₄ = (3 × 4²) + (1 × 4¹) + (2 × 4⁰)
    *   = (3 × 16) + (1 × 4) + (2 × 1)
    *   = 48 + 4 + 2 = **54₁₀**
*   **Step 2: Convert from Base 10 to Base 8.**
    *   54 ÷ 8 = 6 R 6
    *   6 ÷ 8 = 0 R 6
    *   Read bottom-up: **66₈**
*   **Final Answer: 312₄ = 66₈**

**iii) Convert 99₁₀ to Base 2**
*   Use the division-remainder method.
    *   99 ÷ 2 = 49 R 1
    *   49 ÷ 2 = 24 R 1
    *   24 ÷ 2 = 12 R 0
    *   12 ÷ 2 = 6 R 0
    *   6 ÷ 2 = 3 R 0
    *   3 ÷ 2 = 1 R 1
    *   1 ÷ 2 = 0 R 1
*   Read bottom-up: **1100011₂**

---

#### **Question 2(a): Implementing an OR Gate with NAND Gates**

**Expression to Implement: F = A + B**
Using only NAND gates, the process involves a specific arrangement based on De Morgan's laws. The OR function `A+B` is equivalent to `(A' • B')'`.

1.  Create A' using a NAND gate: Tie both inputs of a NAND gate to A. The output is (A•A)' = A'.
2.  Create B' using a NAND gate: Tie both inputs of another NAND gate to B. The output is (B•B)' = B'.
3.  Feed A' and B' into a final NAND gate: The output is (A' • B')'.

**Logic Circuit Diagram:**
```
A --+----[ NAND G1 ]----+
  |                    |
  +--------------------+----[ NAND G3 ]---- F = A+B
                       |
B --+----[ NAND G2 ]----+
  |                    |
  +--------------------+
```

---

#### **Question 2(b): Analyze and Simplify Logic Circuit**

**1. Identify Final Output Expression:**
*   Input A goes into a NOT gate, producing `A'`.
*   Input B goes into a NOT gate, producing `B'`.
*   `A'` and `B'` go into **G1 (AND gate)**, producing `A'B'`.
*   The output of G1 goes into a final **NOT gate**.
*   **Final Expression: F = (A'B')'**

**2. Simplify the Expression:**
*   This expression is a direct application of **De Morgan's Theorem**.
*   **De Morgan's Law states:** `(X • Y)' = X' + Y'`
*   Applying this to our expression:
    *   `F = (A'B')'`
    *   `F = (A')' + (B')'`
*   The double complement law states `X'' = X`.
*   `F = A + B`
*   **Simplified Expression: F = A + B** (This is an OR gate)

**3. Prove with a Truth Table:**

| **A** | **B** | **A'** | **B'** | **A'B'** | **Original F** ( (A'B')' ) | **Simplified F (A+B)** |
| :--- | :-: | :-: | :-: | :---: | :---: | :---: |
| 0 | 0 | 1 | 1 | 1 | **0** | **0** |
| 0 | 1 | 1 | 0 | 0 | **1** | **1** |
| 1 | 0 | 0 | 1 | 0 | **1** | **1** |
| 1 | 1 | 0 | 0 | 0 | **1** | **1** |

**Conclusion:**
The columns for the **Original Expression** and the **Simplified Expression** are identical. This proves that the circuit, which is a NAND gate with inverted inputs, behaves exactly like an OR gate.

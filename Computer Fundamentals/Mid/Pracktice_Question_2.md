### **Practice Midterm Question 02**

**Daffodil International University**
**Department of Software Engineering**
**Midterm Examination, Spring 2025**
**Course Code: SE 111; Course Title: Computer Fundamentals**

**Time: 1 Hour 30 Mins**
**Marks: 25**

**Answer ALL Questions**
---

**1. a)** A cutting-edge research institute is developing a supercomputer designed for complex problem-solving, like natural language processing and expert systems. The computer's architecture is based on Ultra Large-Scale Integration (ULSI) technology and is built for parallel processing to mimic human-like intelligence and reasoning. [Marks-3]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Identify and explain the computer generation from the scenario, detailing its key hardware and software characteristics.**

**b)** When a processor needs to perform an operation, it first looks for the data in a small, extremely fast memory unit integrated directly with or very close to it. If the data isn't there, it retrieves it from the much larger, but slower, main memory. This system significantly boosts the computer's overall speed. [Marks-3]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Compare the two types of computer memory described in the scenario.**

**c)** Perform the following number system conversions, showing all steps: [Marks-9]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; i) Convert **1AD₁₆** to its Base 8 (Octal) equivalent.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ii) Convert **1101.011₂** to its Base 10 (Decimal) equivalent.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; iii) Convert **299₁₀** to its Base 5 equivalent.

---

**2. a)** Illustrate a logic circuit that corresponds to the following Boolean expression: [Marks-3]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**F = (A'B + C)(B' + D)**

**b)** Analyze the logic circuit diagram below to determine its final output expression. After deriving the expression, simplify it using the laws of Boolean algebra. Finally, prove that your simplified expression is correct using a truth table. [Marks-7]

```
A -----------+----[OR G1]----+----[AND G3]---- F (Output)
   |         |              |
B --|>o--+---|----[OR G1]    |
         |   |              |
         +---|--------------+
             |
             +----[AND G2]
             |
C -----------+----[AND G2]

```
*(Note: `|>o--` is a NOT gate, `[OR Gx]` and `[AND Gx]` are OR and AND gates respectively.)*

---

### **Solutions and Detailed Explanations**

#### **Question 1(a): Computer Generation (5th Generation)**

**Answer:**
The generation described is the **Fifth Generation of Computers (1989-Present)**.

**Explanation:**
The keywords in the scenario are "supercomputer," "natural language processing," "expert systems," "Ultra Large-Scale Integration (ULSI)," "parallel processing," and "human-like intelligence" (Artificial Intelligence).

*   **Key Hardware:** This generation is defined by **ULSI (Ultra Large-Scale Integration)** technology, which allows millions of components to be placed on a single microchip. This power enabled the development of powerful microprocessors and the concept of **Parallel Processing**, where multiple CPUs work on different parts of a problem simultaneously. This is essential for building supercomputers.
*   **Key Software Technologies:**
    1.  **Artificial Intelligence (AI):** This is the central theme of the fifth generation. The goal is to create devices that can respond to natural language, learn, and make decisions. Areas like **expert systems**, **natural language processing (NLP)**, and robotics are the focus.
    2.  **Advanced Operating Systems:** The development of sophisticated, user-friendly graphical operating systems for powerful multitasking continued.
    3.  **The Internet and Multimedia:** The World Wide Web became widely accessible, and computers became powerful enough to handle multimedia (sound, images, video) effectively.

**Bengali Meaning (বাংলা অর্থ):**
*   **ULSI (Ultra Large-Scale Integration):** একটি একক চিপে লক্ষ লক্ষ ইলেকট্রনিক উপাদান একত্রিত করার প্রযুক্তি।
*   **Parallel Processing (প্যারালাল প্রসেসিং):** একই সাথে একাধিক প্রসেসর ব্যবহার করে কোনো সমস্যা সমাধান করা।
*   **Artificial Intelligence (AI) (আর্টিফিশিয়াল ইন্টেলিজেন্স):** কৃত্রিম বুদ্ধিমত্তা, যা যন্ত্রকে মানুষের মতো চিন্তা করতে ও শিখতে সাহায্য করে।

**Easy Remember Trick (মনে রাখার কৌশল):**
Fifth generation thinks **"AI & ULSI"**:
*   **A**rtificial **I**ntelligence (main software goal).
*   **ULSI** & Parallel Processing (main hardware technology).

---

#### **Question 1(b): Memory Comparison (Cache vs. Main Memory)**

**Answer:**
The two memory types are **Cache Memory** (the small, fast unit) and **Main Memory/RAM** (the larger, slower unit).

**Comparison:**

| Feature (বৈশিষ্ট্য) | Cache Memory (ক্যাশ মেমোরি) | Main Memory / RAM (প্রধান মেমোরি) |
| :--- | :--- | :--- |
| **Location (অবস্থান)** | Located between the CPU and RAM. It can be directly on the CPU chip (L1/L2 Cache). | It is a separate set of chips on the motherboard, connected to the CPU. |
| **Speed (গতি)** | **Extremely fast.** Its access time is very close to the CPU's processing speed. (অত্যন্ত দ্রুত)। | **Fast, but much slower than cache.** (ক্যাশের চেয়ে অনেক ধীর)। |
| **Size (আকার)** | Very small (e.g., Kilobytes or a few Megabytes). (অনেক ছোট)। | Much larger capacity (e.g., several Gigabytes). (অনেক বড়)। |
| **Cost (খরচ)** | **Very expensive** per byte. | **Less expensive** than cache, but more expensive than secondary storage. |
| **Purpose (উদ্দেশ্য)** | To store frequently used data and instructions to reduce the time the CPU has to wait for data from RAM. | To hold all the data and programs currently being executed by the computer. |

**Easy Remember Trick (মনে রাখার কৌশল):**
*   **Cache** is like your desk drawer: very small and super-fast for frequently needed items.
*   **RAM** is like your bookshelf: larger, holds more, but takes a bit longer to find what you need.

---

#### **Question 1(c): Number System Conversions**

**i) Convert 1AD₁₆ to Base 8**
*   **Step 1 (Hex to 4-bit Binary):**
    *   1₁₆ = 0001₂
    *   A₁₆ (10₁₀) = 1010₂
    *   D₁₆ (13₁₀) = 1101₂
    *   Combined: **0001 1010 1101**
*   **Step 2 (Regroup into 3-bit Binary):**
    *   Starting from the right: **000 110 101 101**
*   **Step 3 (3-bit Binary to Octal):**
    *   000₂ = 0₈
    *   110₂ = 6₈
    *   101₂ = 5₈
    *   101₂ = 5₈
    *   **Final Answer: 0655₈ or simply 655₈**

**ii) Convert 1101.011₂ to Base 10**
*   **Integer Part (1101):**
    *   (1×2³) + (1×2²) + (0×2¹) + (1×2⁰) = 8 + 4 + 0 + 1 = **13**
*   **Fractional Part (.011):**
    *   (0×2⁻¹) + (1×2⁻²) + (1×2⁻³) = 0 + (1/4) + (1/8) = 0 + 0.25 + 0.125 = **0.375**
*   **Combine:** 13 + 0.375 = **13.375₁₀**

**iii) Convert 299₁₀ to Base 5**
*   Use the division-remainder method.

| Division | Quotient | Remainder |
| :--- | :--- | :---: |
| 299 ÷ 5 | 59 | 4 |
| 59 ÷ 5 | 11 | 4 |
| 11 ÷ 5 | 2 | 1 |
| 2 ÷ 5 | 0 | 2 |

*   Read the remainders from bottom to top: **2144₅**

---

#### **Question 2(a): Illustrate Logic Circuit**

**Expression: F = (A'B + C)(B' + D)**
1.  **A'**: Input A goes through a **NOT** gate.
2.  **A'B**: Output of A' and input B go into an **AND** gate.
3.  **A'B + C**: Output of the AND gate and input C go into an **OR** gate.
4.  **B'**: Input B goes through a **NOT** gate.
5.  **B' + D**: Output of B' and input D go into another **OR** gate.
6.  **Final F**: The outputs from the two OR gates (step 3 and step 5) go into a final **AND** gate.

---

#### **Question 2(b): Analyze and Simplify Logic Circuit**

**1. Identify Final Output Expression:**
*   **G1 (OR Gate):** Inputs are A and B'. Output = `A + B'`
*   **G2 (AND Gate):** Inputs are B' and C. Output = `B'C`
*   **G3 (Final AND Gate):** Inputs are outputs from G1 and G2.
*   **Final Expression: F = (A + B')(B'C)**

**2. Simplify the Expression:**
*   `F = (A + B')(B'C)`
*   `F = A(B'C) + B'(B'C)` *(Distributive Law)*
*   `F = AB'C + (B'B')C`
*   `F = AB'C + B'C` *(Idempotent Law: B'B' = B')*
*   `F = B'C (A + 1)` *(Take B'C as common - Distributive Law)*
*   Since `A + 1 = 1` *(Annulment Law)*,
*   `F = B'C • 1`
*   **Simplified Expression: F = B'C**

**3. Prove with a Truth Table:**
We need to prove that `(A + B')(B'C)` is the same as `B'C`.

| **A** | **B** | **C** | **B'** | **A + B'** (G1) | **B'C** (G2) | **Original F** (G1•G2) | **Simplified F (B'C)** |
| :--- | :-: | :-: | :-: | :---: | :---: | :---: | :---: |
| 0 | 0 | 0 | 1 | 1 | 0 | **0** | **0** |
| 0 | 0 | 1 | 1 | 1 | 1 | **1** | **1** |
| 0 | 1 | 0 | 0 | 0 | 0 | **0** | **0** |
| 0 | 1 | 1 | 0 | 0 | 0 | **0** | **0** |
| 1 | 0 | 0 | 1 | 1 | 0 | **0** | **0** |
| 1 | 0 | 1 | 1 | 1 | 1 | **1** | **1** |
| 1 | 1 | 0 | 0 | 1 | 0 | **0** | **0** |
| 1 | 1 | 1 | 0 | 1 | 0 | **0** | **0** |

**Conclusion:**
The columns for **Original F** and **Simplified F** are identical, confirming the simplification is correct.

### **Practice Midterm Question 05**

**Daffodil International University**
**Department of Software Engineering**
**Midterm Examination, Spring 2025**
**Course Code: SE 111; Course Title: Computer Fundamentals**

**Time: 1 Hour 30 Mins**
**Marks: 25**

**Answer ALL Questions**
---

**1. a)** A university's computer science department from the early 1970s used a "minicomputer" to serve multiple students at once. This machine was built using **Integrated Circuits (ICs)**, making it much smaller and more reliable than its predecessors. It ran a **timesharing operating system**, allowing students to connect and run programs simultaneously from different **terminals**. [Marks-3]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**From the details provided, identify and describe this computer generation, including its signature hardware and software innovations.**

**b)** An embedded systems engineer is choosing non-volatile memory for three different devices:
    1.  A pocket calculator where the core software will be written once during manufacturing and never changed.
    2.  A video game cartridge in development, where the team needs to erase and rewrite the firmware many times by removing the chip and exposing it to a special light.
    3.  A modern Wi-Fi router that must receive and install firmware updates over the internet without being opened.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Identify and briefly compare the three specific types of ROM best suited for each of these scenarios.** [Marks-3]

**c)** Perform the following number system conversions, clearly showing your work: [Marks-9]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; i) Convert **6AD.C₁₆** to its Base 8 (Octal) equivalent.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ii) Convert **1120₃** to its Base 9 equivalent using a shortcut method.
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; iii) Convert **75.25₁₀** to its Base 8 (Octal) equivalent.

---

**2. a)** The NOR gate is known as a universal gate. **Using ONLY two-input NOR gates**, draw the logic circuit that performs the function of a standard two-input AND gate (F = A • B). [Marks-3]

**b)** For the logic circuit shown below:
    1.  Write down the final Boolean expression for the output F.
    2.  Use Boolean algebra laws to simplify the expression to its simplest form.
    3.  Construct a truth table to prove that the original and simplified expressions are equivalent. [Marks-7]

```
A --|>o---+----[ AND G1 ]----+
       |   |                 |
       |   +-----------------|----[ OR G2 ]---- F (Output)
       |                     |
B -----+-----[ AND G1 ]
```
*(Diagram: Input A goes into a NOT gate. The output A' is fed into one input of AND gate G1 AND one input of OR gate G2. Input B is fed into the other input of G1. The output of G1 is fed into the other input of G2.)*

---

### **Solutions and Detailed Explanations**

#### **Question 1(a): Computer Generation (3rd Generation)**

**Answer:**
The scenario describes the **Third Generation of Computers (1964-1975)**.

**Explanation:**
The keywords are definitive for this era: **Integrated Circuits (ICs)**, **minicomputers**, and **timesharing operating systems**.

*   **Key Hardware:** The move from transistors to **Integrated Circuits (ICs)** was the landmark hardware innovation. ICs placed many transistors, resistors, and capacitors on a single silicon chip, drastically increasing speed and reliability while reducing size and cost. This led to the creation of **minicomputers** (like the PDP-8), which were smaller and cheaper than mainframes.
*   **Key Software Technologies:**
    1.  **Operating Systems with Multiprogramming:** This generation saw the rise of sophisticated operating systems that could manage multiple programs at once.
    2.  **Timesharing:** This feature allowed multiple users to interact with a single computer simultaneously through **terminals**, creating the illusion that each user had exclusive use of the machine. This greatly improved programmer productivity.
    3.  **Unbundling:** The practice of selling hardware and software separately began, which gave birth to the modern software industry.

**Bengali Meaning (বাংলা অর্থ):**
*   **Integrated Circuit (IC) (ইন্টিগ্রেটেড সার্কিট):** একটি একক চিপ যাতে অনেকগুলো ট্রানজিস্টর থাকে।
*   **Minicomputer (মিনি কম্পিউটার):** মেইনফ্রেমের চেয়ে ছোট এবং সাশ্রয়ী কম্পিউটার।
*   **Timesharing (টাইম-শেয়ারিং):** একটি অপারেটিং সিস্টেমের বৈশিষ্ট্য যা একাধিক ব্যবহারকারীকে একই সময়ে একটি কম্পিউটার ব্যবহার করতে দেয়।

**Easy Remember Trick (মনে রাখার কৌশল):**
3rd Gen = **"I See Time Sharing!"**
*   **IC** (Integrated Circuit)
*   **Time Sharing** OS for many users.

---

#### **Question 1(b): Specific Types of ROM**

**Answer:**
The three types of ROM are:
1.  For the calculator: **PROM (Programmable Read-Only Memory)**
2.  For the game cartridge: **EPROM (Erasable Programmable Read-Only Memory)**
3.  For the router: **EEPROM (Electrically Erasable Programmable Read-Only Memory)**

**Comparison:**

| Feature | PROM (for Calculator) | EPROM (for Game Cartridge) | EEPROM (for Router) |
| :--- | :--- | :--- | :--- |
| **Programmability** | Can be programmed **once** by the user/manufacturer. Cannot be erased. | Can be erased and reprogrammed **many times**. | Can be erased and reprogrammed **many times**. |
| **Erasing Method** | **Not possible** to erase. | Must be removed from the circuit and exposed to **Ultraviolet (UV) light**. | Can be erased **electrically** while still in the circuit. No removal needed. |
| **Flexibility** | Lowest flexibility (write-once). | Good for development, but erasing is inconvenient. | Highest flexibility; allows for easy "in-field" updates. |

---

#### **Question 1(c): Number System Conversions**

**i) Convert 6AD.C₁₆ to Base 8**
*   **Step 1 (Hex to 4-bit Binary):**
    *   6₁₆ = 0110₂
    *   A₁₆ (10) = 1010₂
    *   D₁₆ (13) = 1101₂
    *   C₁₆ (12) = 1100₂
    *   Combined Binary: **0110 1010 1101 . 1100**
*   **Step 2 (Regroup into 3-bit sections):**
    *   Integer part (from right): `011 010 101 101`
    *   Fractional part (from left): `110 000` (add trailing zeros)
*   **Step 3 (3-bit Binary to Octal):**
    *   011₂ = 3₈; 010₂ = 2₈; 101₂ = 5₈; 101₂ = 5₈
    *   110₂ = 6₈; 000₂ = 0₈
    *   **Final Answer: 3255.6₈**

**ii) Convert 1120₃ to Base 9**
*   Since 9 = 3², we can group the base-3 digits in pairs from the right and convert each pair.
*   Group `1120₃` into `(11)₃` and `(20)₃`.
*   Convert each pair to decimal to find the base-9 digit:
    *   `(11)₃` = (1 × 3¹) + (1 × 3⁰) = 3 + 1 = **4**₁₀
    *   `(20)₃` = (2 × 3¹) + (0 × 3⁰) = 6 + 0 = **6**₁₀
*   **Final Answer: 46₉**

**iii) Convert 75.25₁₀ to Base 8**
*   **Integer Part (75):** Use division-remainder.
    *   75 ÷ 8 = 9 R 3
    *   9 ÷ 8 = 1 R 1
    *   1 ÷ 8 = 0 R 1
    *   Integer Part (bottom-up): **113₈**
*   **Fractional Part (0.25):** Use repeated multiplication.
    *   0.25 × 8 = **2**.00
    *   Fractional Part (top-down): **.2₈**
*   **Combine:** **113.2₈**

---

#### **Question 2(a): Implementing an AND Gate with NOR Gates**

**Expression to Implement: F = A • B**
From De Morgan's Law, `A•B` is equivalent to `(A' + B')'`. We can build this using only NOR gates.
1.  Create A': Use a NOR gate with both inputs tied to A. The output is (A+A)' = A'.
2.  Create B': Use a NOR gate with both inputs tied to B. The output is (B+B)' = B'.
3.  Feed A' and B' into a final NOR gate: The output is (A' + B')', which equals A'' • B'' = A • B.

**Logic Circuit Diagram:**
```
A --+----[ NOR G1 ]----+
  |                    |
  +--------------------+----[ NOR G3 ]---- F = A•B
                       |
B --+----[ NOR G2 ]----+
  |                    |
  +--------------------+
```

---

#### **Question 2(b): Analyze and Simplify Logic Circuit**

**1. Identify Final Output Expression:**
*   Input A is inverted to produce `A'`.
*   **G1 (AND Gate):** Inputs are `A'` and `B`. Output = `A'B`.
*   **G2 (OR Gate):** Inputs are the output from G1 (`A'B`) and the inverted input `A'`.
*   **Final Expression: F = A' + A'B**

**2. Simplify the Expression:**
*   `F = A' + A'B`
*   `F = A'(1 + B)`  *(Factor out A' using the Distributive Law)*
*   By the Annulment Law, `1 + X = 1`. Therefore, `1 + B = 1`.
*   `F = A'(1)`
*   `F = A'`  *(Identity Law)*
*   This is an application of the **Absorption Law:** `X + XY = X`. Here, X = A'.
*   **Simplified Expression: F = A'**

**3. Prove with a Truth Table:**

| **A** | **B** | **A'** | **A'B** (G1) | **Original F** ( A' + A'B ) | **Simplified F (A')** |
| :--- | :-: | :-: | :---: | :---: | :---: |
| 0 | 0 | 1 | 0 | **1** | **1** |
| 0 | 1 | 1 | 1 | **1** | **1** |
| 1 | 0 | 0 | 0 | **0** | **0** |
| 1 | 1 | 0 | 0 | **0** | **0** |

**Conclusion:**
The columns for the **Original Expression** and the **Simplified Expression** are perfectly identical, confirming that the entire circuit simplifies down to just a single NOT gate for input A.

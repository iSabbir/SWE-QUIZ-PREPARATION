---

---
title: "Question 1(a): BMI Classification — Algorithm & Flowchart"
---

### **Given**

BMI formula:

\[
\text{BMI} = \frac{\text{Weight (kg)}}{(\text{Height (m)})^2}
\]

### **BMI Categories**

* **Underweight:** BMI < 18.5
* **Healthy Weight:** 18.5 ≤ BMI ≤ 24.9
* **Overweight:** 25 ≤ BMI ≤ 29.9
* **Obese:** BMI ≥ 30

---

## ✅ **Algorithm (Pseudo Code)**

```
START
INPUT height, weight
BMI = weight / (height * height)

IF BMI < 18.5 THEN
    PRINT "Underweight"
ELSE IF BMI >= 18.5 AND BMI <= 24.9 THEN
    PRINT "Healthy Weight"
ELSE IF BMI >= 25 AND BMI <= 29.9 THEN
    PRINT "Overweight"
ELSE
    PRINT "Obese"
END IF

END
```

---

## ✅ **Flowchart (Exam-friendly)**

```
 START
   |
Input Height, Weight
   |
BMI = weight / (height²)
   |
BMI < 18.5 ?
   |Yes → Underweight
   |No
BMI ≤ 24.9 ?
   |Yes → Healthy
   |No
BMI ≤ 29.9 ?
   |Yes → Overweight
   |No → Obese
   |
  END
```

---

### 📝 **Bangla Notes**

* BMI দিয়ে শরীরের ওজনের অবস্থা বোঝা হয়
* Height **meter** এ নিতে হবে
* Formula ভুল লিখলে পুরো marks যাবে
* Condition গুলো **ascending order** এ লিখলে logic clear হয়

---

# **Question 1(b): C Code Error Detection + Correction + Output (7 marks)**

### **Given Code (Errors present)** 

### ❌ **Detected Errors (write at least 7)**

1. `#Include` ❌ → `#include`
2. `<studio.h>` ❌ → `<stdio.h>`
3. `INT main()` ❌ → `int main()`
4. `print()` ❌ → `printf()`
5. `scan()` ❌ → `scanf("%d",&num)`
6. `if (num % 3 = 0 || num % 5 = 0);`

   * `=` ❌ should be `==`
   * extra `;` ❌ breaks logic
7. `prnt()` ❌ → `printf()`
8. Missing semicolons `;`
9. `ret 0;` ❌ → `return 0;`

---

## ✅ **Corrected C Program**

```c
#include <stdio.h>

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    if (num % 3 == 0 && num % 5 == 0) {
        printf("The number is divisible by both 3 and 5\n");
    } else {
        printf("The number is not divisible by both 3 and 5\n");
    }

    return 0;
}
```

---

## ✅ **Expected Output**

### **Input: 15**

* 15 divisible by 3 and 5
  **Output:**
  `The number is divisible by both 3 and 5`

### **Input: 10**

* 10 divisible by 5 but not 3
  **Output:**
  `The number is not divisible by both 3 and 5`

---

### 📝 **Bangla Notes**

* `=` মানে assign, `==` মানে compare
* `if(condition);` দিলে condition কাজ করে না
* `scanf` তে **&** না দিলে input নেয় না

---

# **Question 1(c): Database Keys Identification (5 marks)**

### **Tables Given**

* **Student(StudentID, Name, Age, CGPA, CourseID)**
* **Course(CourseID, CourseName, Credit)** 

---

## ✅ **Two Most Important Keys**

### 🔑 **Primary Key**

* **Student Table:** `StudentID`
* **Course Table:** `CourseID`
* Unique & cannot be NULL

### 🔑 **Foreign Key**

* `CourseID` in **Student Table**
* References `CourseID` in **Course Table**

---

## ✅ **Difference**

| Primary Key                  | Foreign Key          |
| ---------------------------- | -------------------- |
| Uniquely identifies a record | Creates relationship |
| Cannot repeat                | Can repeat           |
| Cannot be NULL               | Can be NULL          |

---

### 📝 **Bangla Notes**

* Primary Key = একক পরিচয়
* Foreign Key = দুই টেবিলের connection
* CourseID দিয়ে Student ↔ Course link হয়

---

# **Question 1(d): Network Topology Identification (5 marks)**

---

## **Scenario 1**

> All devices connect to a central hub with a backup hub. If both fail, network stops. 

### ✅ **Answer: STAR Topology**

**Reason**

* Central hub controls communication
* Backup hub = redundancy
* Hub failure = network down

```
      PC
       |
PC — HUB — PC
       |
      PC
```

---

## **Scenario 2**

> Each device connects to every other device; reliable but costly. 

### ✅ **Answer: MESH Topology**

**Reason**

* Multiple connections
* High reliability
* Expensive & complex

```
PC1 ---- PC2
 |  \   /  |
 |   \ /   |
 |   / \   |
 |  /   \  |
PC3 ---- PC4
```

---

### 📝 **Bangla Notes**

* Star = hub based
* Mesh = সবাই সবার সাথে connected
* Mesh costly but fault-tolerant

---

# **Question 2(a): Identify Vulnerabilities from Stories (5 marks)**

---

## **Story 1**

Script injected in comment section:

```html
<script>alert("Hacked")</script>
```

### ✅ **Vulnerability: Cross-Site Scripting (XSS)**

**Explanation**

* Malicious script runs in browser
* Can steal cookies/session

---

## **Story 2**

Input:

```sql
101'; DROP TABLE patients; --
```

### ✅ **Vulnerability: SQL Injection**

**Explanation**

* SQL command injected
* Deletes database data

---

### 📝 **Bangla Notes**

* XSS → browser attack
* SQL Injection → database attack
* Both happen due to **no input validation**

---

# **Question 2(b): Secure Telemedicine Technology (5 marks)**

### **Scenario Summary**

* Data stored & sent securely
* Only authorized doctors can read
* Intercepted data remains unreadable
* Data transformed into secure form 

---

## ✅ **Technology: Encryption (Asymmetric Encryption)**

### **How it Works (Step-by-Step)**

1. Doctor has **Public Key & Private Key**
2. Data encrypted using **Public Key**
3. Only **Private Key** can decrypt
4. Interceptor cannot read data

---

### **Diagram**

```
Patient Data
   |
Encrypt with Doctor's Public Key
   |
Encrypted Data (Ciphertext)
   |
Decrypt with Doctor's Private Key
   |
Doctor Reads Data
```

---

### 📝 **Bangla Notes**

* Encryption = data lock করা
* Asymmetric = Public + Private key
* Intercept হলেও data safe থাকে

---

## ✅ **Final Tip for Exam**

* Headings + diagrams = bonus marks
* Bangla explanation helps **clarity in viva & scripts**
* Logic > code length

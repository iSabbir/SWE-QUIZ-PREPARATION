---

# 1(a) Salary Calculation System — Algorithm + Flowchart (15 marks)

**Question summary:** You must calculate **monthly salary** by:

* **Adding allowances**: Rent, Medical (with base salary)
* **Deducting**: tax, provident fund, other expenses
* **Adding bonus** based on performance rating:

  * **10%** if rating **≥ 8**
  * **20%** if rating **between 5 and 7**
  * **0%** if rating **< 5** 

## ✅ Step-by-step formula (write in exam)

Let:

* `BS` = Base Salary
* `RA` = Rent Allowance
* `MA` = Medical Allowance
* `TAX`, `PF`, `OE` = Tax, Provident Fund, Other Expenses
* `R` = Performance Rating

**Gross Salary** = `BS + RA + MA`
**Total Deduction** = `TAX + PF + OE`
**Bonus**:

* if `R >= 8` → `Bonus = 0.10 * BS`
* else if `5 <= R <= 7` → `Bonus = 0.20 * BS`
* else → `Bonus = 0`

**Net Salary** = `Gross Salary - Total Deduction + Bonus`

## ✅ Algorithm (Pseudo Code)

```text
START
INPUT BS, RA, MA
INPUT TAX, PF, OE
INPUT R

GROSS = BS + RA + MA
DEDUCT = TAX + PF + OE

IF R >= 8 THEN
    BONUS = 0.10 * BS
ELSE IF R >= 5 AND R <= 7 THEN
    BONUS = 0.20 * BS
ELSE
    BONUS = 0
END IF

NET = GROSS - DEDUCT + BONUS
PRINT NET

END
```

## ✅ Flowchart (copyable)

```text
  ┌─────────┐
  │ START   │
  └────┬────┘
       │
       v
┌──────────────────────┐
│ Input BS, RA, MA      │
└─────────┬────────────┘
          │
          v
┌──────────────────────┐
│ Input TAX, PF, OE, R  │
└─────────┬────────────┘
          │
          v
┌──────────────────────┐
│ GROSS = BS+RA+MA       │
│ DEDUCT = TAX+PF+OE     │
└─────────┬────────────┘
          │
          v
     ┌────────────┐
     │ R >= 8 ?    │
     └───┬────┬───┘
        Yes   No
         │     │
         v     v
 ┌────────────┐  ┌──────────────────┐
 │BONUS=0.10BS│  │ 5<=R<=7 ?         │
 └─────┬──────┘  └───┬────────┬─────┘
       │            Yes       No
       │             │         │
       v             v         v
                  ┌──────────┐ ┌─────────┐
                  │BONUS=0.20│ │BONUS=0  │
                  │   *BS    │ └────┬────┘
                  └────┬─────┘      │
                       └──────┬──────┘
                              v
                 ┌──────────────────────┐
                 │ NET=GROSS-DEDUCT+BONUS│
                 │ Print NET             │
                 └─────────┬────────────┘
                           v
                       ┌──────┐
                       │ END  │
                       └──────┘
```

### 📝 Bangla Notes (easy marks booster)

* **Gross Salary = বেস + Rent + Medical**
* **Deduction = Tax + PF + Others**
* **Net = Gross − Deduction + Bonus**
* Bonus ট্রিক:

  * **8+ → 10%**
  * **5–7 → 20%**
  * **<5 → 0%**
* Bonus **Base Salary এর উপর** হিসাব করবে (Allowance এর উপর না লিখলে safe)

---

# 1(b) C Code — Find errors + Correct code + Output for 20, 7, 10 (5 marks)

The given code has many syntax mistakes (wrong keywords, wrong scanf/printf, wrong conditions, extra semicolons, etc.). 

## ✅ Common errors (write these points)

1. `#Include` → must be `#include`
2. `<studio,h>` → must be `<stdio.h>`
3. `INT main()` → should be `int main()`
4. `print()` → should be `printf()`
5. `scan("%d" num);` → should be `scanf("%d", &num);`
6. `if (num % 2 = 0 && num > 10);`

   * `=` should be `==`
   * extra `;` after if (kills the condition)
7. `printl()` / `prnt()` → should be `printf()`
8. `else if (num % 2 = 1)` → should be `== 1`
9. Missing semicolons in print statements
10. Wrong return value (`return 1;` should be `return 0;`)

## ✅ Corrected C Program (standard, clean)

```c
#include <stdio.h>

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    if (num % 2 == 0 && num > 10) {
        printf("The number is even and greater than 10\n");
    } 
    else if (num % 2 == 1) {
        printf("The number is odd\n");
    } 
    else {
        printf("The number is even and less than or equal to 10\n");
    }

    return 0;
}
```

## ✅ Expected Output

### Input: 20

* 20 is even and > 10
  **Output:** `The number is even and greater than 10`

### Input: 7

* 7 is odd
  **Output:** `The number is odd`

### Input: 10

* 10 is even and NOT > 10 (so else case)
  **Output:** `The number is even and less than or equal to 10`

### 📝 Bangla Notes

* `scanf("%d",&num)` → **& না দিলে ইনপুট নেয় না**
* `=` মানে assign, `==` মানে compare
* `if(condition);` দিলে condition কাজই করবে না (সবসময় block চলবে)

---

# 1(c) Identify Topology + Reason + Diagram (5 marks)

Two scenarios are given. 

## Scenario–1

**Clue:** “single central cable backbone… data travels along the cable… if main cable fails entire network stops” 
✅ **Answer: BUS Topology**

### Reason

* One main cable (backbone)
* All devices tap into it
* Backbone fails → whole network down

### Diagram (Bus)

```text
 PC1   PC2   PC3   PC4
  |     |     |     |
========================   (Backbone cable)
```

## Scenario–2

**Clue:** “devices placed within close range and connected to each other… costly” 
✅ **Answer: MESH Topology** (costly because many links/cables)

### Reason

* Devices are interconnected
* More cables + ports needed → expensive

### Diagram (Mesh)

```text
   PC1------PC2
    |\      /|
    | \    / |
    |  \  /  |
    |   \/   |
    |   /\   |
    |  /  \  |
    | /    \ |
    |/      \|
   PC3------PC4
```

### 📝 Bangla Notes

* **Bus = একটাই main wire → wire কাটলে সব বন্ধ**
* **Mesh = সবাই সবার সাথে connected → costly কিন্তু reliable**

---

# 1(d) DBMS Technique to reduce duplication & update problems (5 marks)

The institute keeps student, course, instructor data in **one table**, causing:

* repeated data
* inconsistencies
* hard updates
* inefficient management 

✅ **Best technique: Normalization (1NF → 2NF → 3NF)**

## Why Normalization fits perfectly

Normalization:

* removes redundancy (duplicate info)
* prevents update anomalies
* ensures consistency
* makes updates easy by splitting into related tables

## Proper design (example decomposition)

Instead of one huge table, split like:

**Student(StudentID, Name, Dept, …)**
**Course(CourseID, CourseName, Credit, …)**
**Instructor(InstructorID, InstructorName, …)**
**Enrollment(StudentID, CourseID, Semester, …)**
**Teaches(InstructorID, CourseID, …)**

### 📝 Bangla Notes

* Normalization মানে **ডাটাকে ভাগ করে clean করা**
* এক টেবিলে সব রাখলে:

  * same course name বারবার
  * instructor change হলে অনেক row update করতে হয়
* ভাগ করলে update easy + duplication কমে

---

# 2(a) Vulnerability type + prevention (5 marks)

Scenario: user inputs are not validated; attacker enters **malicious commands**, application executes them → unauthorized actions and data access. 

✅ **Vulnerability: Injection Attack (Most commonly SQL Injection)**

## Why it is SQL Injection (exam logic)

* “input fields”
* “malicious commands”
* “application executes”
* “access sensitive information”
  This strongly matches SQL injection behavior.

## Prevention (write these for full marks)

1. **Input Validation & Sanitization**
2. **Parameterized Queries / Prepared Statements** (no string concatenation)
3. **Escape special characters** (as extra layer)
4. **Least privilege DB account** (no admin DB user)
5. **Use ORM / secure query builder**
6. **Error handling** (don’t show SQL errors to users)
7. **WAF / Security testing** (optional extra)

### 📝 Bangla Notes

* SQL Injection = input box এ SQL ঢুকিয়ে DB manipulate করা
* Best fix = **Prepared Statement** + **Validation**

---

# 2(b) Identify technology in Brain Station app + How it works + diagram (5 marks)

Scenario says:

* Enosis “Let’s Talk” uses **shared secret key** → symmetric encryption
* Brain Station uses **separate keys for sender and receiver** → stronger security
* Passwords stored as **fixed-length hashes** 

✅ **Technology in Brain Station chat app: Asymmetric Encryption (Public Key Cryptography)**
Also mentions: ✅ **Hashing for password storage**

## How Asymmetric Encryption works (simple but full-mark)

* Each user has:

  * **Public Key** (shared with others)
  * **Private Key** (kept secret)
* Sender encrypts message using receiver’s **public key**
* Only receiver can decrypt using their **private key**

### Diagram (Asymmetric encryption)

```text
Sender (A)                           Receiver (B)
---------                           ------------
Message: "Hi" 
   |
Encrypt using B's PUBLIC KEY  ----->  Ciphertext
                                     |
                               Decrypt using B's PRIVATE KEY
                                     |
                                  "Hi"
```

## Password protection part (Hashing)

* Password is converted into a **fixed-length hash** (e.g., SHA-256)
* Hash is stored (not original password)
* During login, entered password is hashed again and compared

### Hashing diagram

```text
Password --> Hash Function --> Fixed-length Hash --> Store in DB
Login: input password --> hash --> compare with stored hash
```

### 📝 Bangla Notes

* Symmetric = **same key encrypt/decrypt**
* Asymmetric = **Public key encrypt, Private key decrypt**
* Hashing = password **উল্টানো যায় না**, শুধু compare করা যায়

---

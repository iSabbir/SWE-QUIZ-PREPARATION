---

## 1(a) Algorithm (Pseudo code) + Flowchart (Nila’s coding time)

**Problem meaning (deeply):**
Input = **hours of raining (R)**.
Output = **hours of coding** or **“Sleep”**.

Rules from question: 

* If **R = 0** → output **Sleep**
* Else if **R > 12** → output **Sleep**
* Else if **R is even** → coding = **2 × R**
* Else (**R is odd**) → coding = **3 × R**

### ✅ Pseudo Code (exam-ready)

```
START
INPUT R

IF R == 0 THEN
    PRINT "Sleep"
ELSE IF R > 12 THEN
    PRINT "Sleep"
ELSE
    IF R % 2 == 0 THEN
        C = 2 * R
        PRINT C
    ELSE
        C = 3 * R
        PRINT C
    ENDIF
ENDIF

END
```

### ✅ Flowchart (text/ASCII version you can copy in exam)

```
   ┌─────────┐
   │ START   │
   └────┬────┘
        │
        v
   ┌───────────────┐
   │ Input R (rain)│
   └────┬──────────┘
        │
        v
   ┌───────────────┐
   │  R == 0 ?      │
   └───┬───────┬───┘
      Yes     No
       │       │
       v       v
┌──────────┐  ┌───────────────┐
│ Print    │  │   R > 12 ?      │
│ "Sleep"  │  └───┬───────┬───┘
└────┬─────┘     Yes     No
     │            │       │
     v            v       v
  ┌───────┐  ┌──────────┐  ┌───────────────┐
  │  END  │  │ Print    │  │  R even?       │
  └───────┘  │ "Sleep"  │  └───┬───────┬───┘
             └────┬─────┘     Yes     No
                  │            │       │
                  v            v       v
               ┌───────┐  ┌────────┐ ┌────────┐
               │ END   │  │ C=2*R  │ │ C=3*R  │
               └───────┘  └───┬────┘ └───┬────┘
                              │          │
                              v          v
                         ┌────────┐  ┌────────┐
                         │ Print C│  │ Print C│
                         └───┬────┘  └───┬────┘
                             │           │
                             v           v
                           ┌──────────────┐
                           │     END      │
                           └──────────────┘
```

### 📝 Bangla Notes (easy memorizing)

* **R=0 বা R>12 হলে → Sleep** (কোডিং নাই)
* **জোড় (even) হলে → 2×R**
* **বিজোড় (odd) হলে → 3×R**
* মনে রাখার ট্রিক:

  * **Even = 2 (জোড় মানে ডাবল)**
  * **Odd = 3 (বিজোড় মানে ট্রিপল)**
  * **0/Over 12 = Sleep (বৃষ্টি নাই বা বেশি হলে ঘুম)**

---

## 1(b) Find the existing errors in the given C code + corrected version

The code shown has multiple syntax + logical + library issues. 

### ✅ Errors (write these in exam for full marks)

1. `int main()` এর পরে `{` missing / wrong bracket structure (code is inconsistent).
2. `int temperature = 30` → **semicolon missing** (`;`)
3. `float threshold = 25;` OK, but next line:
4. `difference = temperature - threshold;`

   * **difference variable declared নাই**
   * also type should be `float` (because threshold float)
5. `/Temperature Alert/` is invalid comment.

   * C comment should be `// ...` or `/* ... */`
6. `if differencc > 0`

   * variable name typo: `differencc` vs `difference`
7. `printf(...)` lines missing semicolon `;`
8. `clrscr` is wrong:

   * should be `clrscr();` but **it’s non-standard**, needs `conio.h`, and many compilers don’t support it.
9. `for (i = 0; i < 10; i++)`

   * **i declared নাই** (`int i;`)
10. `printf("Iteration: %d\n", i)` missing semicolon `;`
11. Braces `{ }` placement is broken (if/else/for blocks not properly closed).

### ✅ Corrected C Program (clean + standard)

```c
#include <stdio.h>

int main() {
    int temperature = 30;
    float threshold = 25.0f;
    float difference = temperature - threshold;

    printf("Temperature Alert!\n");

    if (difference > 0) {
        printf("Temperature is above threshold\n");
    } else {
        printf("Temperature is below threshold\n");
    }

    for (int i = 0; i < 10; i++) {
        printf("Iteration: %d\n", i);
    }

    return 0;
}
```

### 📝 Bangla Notes (quick understanding)

* **Semicolon (;)** না দিলে C code ভেঙে যায়
* Variable আগে **declare** করতে হয় (difference, i)
* Comment লিখতে হয়: `//` বা `/* */`
* Typo (বানান ভুল) হলে compiler variable চিনতে পারে না
* `clrscr()` অনেক সময় কাজ করে না (non-standard), তাই exam এ standard রাখাই safe

---

## 1(c) Relate at least four keys from the given tables + explain

Two tables are given: 

* **Employee table**: EmpId, EmpName, EmpLicense, EmpPassport, DId
* **Department table**: DId, Designation

### ✅ Keys & Relationships (minimum 4)

1. **Primary Key (Employee table): EmpId**

   * Unique for each employee (1001, 1002, …)

2. **Primary Key (Department table): DId**

   * Unique for each designation (1..5)

3. **Foreign Key (Employee table): DId**

   * Employee’s DId points to Department table’s DId
   * Meaning: Employee কোন designation এ আছে, সেটা map করে

4. **Relationship (One-to-Many): Department → Employees**

   * One designation (like Manager = DId 4) can have many employees
   * Example: DId=4 appears for multiple employees → same designation

**Also you can mention (extra for marks):**

* EmpLicense / EmpPassport are candidate keys only if unique (depends on constraints), but EmpId is guaranteed unique.

### 📝 Bangla Notes

* **Primary Key = ইউনিক আইডি** (একবারই থাকবে)
* **Foreign Key = অন্য টেবিলের Primary Key কে রেফার করে**
* **One-to-Many = ১টা ডিপার্টমেন্টে অনেক কর্মী হতে পারে**
* DId দিয়ে employee ↔ designation connect হয় (join concept)

---

## 2) Network category analysis for the university scenario (LAN, MAN, WAN, PAN)

Scenario says: multiple buildings across campus + classrooms/labs/admin + centralized resources + online platforms + conferences worldwide. 
So, **one single network type is not enough** — it’s a combination.

### ✅ Best mapping (exam-perfect)

1. **LAN (Local Area Network) — inside each building**

* Each building (classrooms, labs, admin office) should have its own LAN.
* Uses: switches, Ethernet, Wi-Fi APs
* Purpose: fast internal communication (PC to server, lab devices, printers)

2. **MAN / Campus Backbone (acts like MAN) — connects buildings داخل ক্যাম্পাস**

* The campus itself connects multiple LANs using fiber backbone.
* This is commonly called a **Campus Area Network (CAN)**, but in your given options it fits best under **MAN-style** coverage.
* Purpose: inter-building communication, central database access, internal services

3. **WAN — for global connectivity (internet + remote users)**

* Online learning platforms, cloud services, global conference participants → WAN needed.
* WAN is basically Internet/ISP links + VPN + firewall routing.
* Purpose: connect to the world.

4. **PAN — personal devices near a user**

* Students/professors connecting phone, smartwatch, earbuds, laptop hotspot, Bluetooth, etc.
* Purpose: short-range personal connectivity.

### ✅ Suggested final design statement (write in exam)

* “Each building uses **LAN**, all building LANs are connected through a high-speed **campus backbone (MAN/CAN)**, and the campus connects to external services via **WAN** (Internet). Individual user devices form **PAN** around each person.”

### 📝 Bangla Notes (easy)

* **LAN = এক বিল্ডিং/এক ফ্লোরের নেটওয়ার্ক**
* **MAN/CAN = পুরো ক্যাম্পাসে বিল্ডিংগুলোকে fiber দিয়ে কানেক্ট**
* **WAN = ইন্টারনেট/বিশ্বের সাথে কানেকশন**
* **PAN = একজন মানুষের কাছাকাছি ডিভাইস (Bluetooth/Hotspot)**

---


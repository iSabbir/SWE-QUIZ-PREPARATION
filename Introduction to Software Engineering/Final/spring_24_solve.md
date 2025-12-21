### Solve 1:

---

### **Question 1**

#### **1(a) Describe various methods of Black box testing, providing an example for each technique. (5 Marks)**
**সমাধান:**
Black Box Testing হলো এমন একটি টেস্টিং পদ্ধতি যেখানে সফটওয়্যারের ইন্টারনাল কোড বা ডিজাইন না দেখে শুধুমাত্র ইনপুট এবং আউটপুট চেক করা হয়।

*   **Equivalence Partitioning (EP):** ইনপুট ডেটাকে কয়েকটি গ্রুপে ভাগ করা হয়। যেমন: একটি ফিল্ড ১-১০০ গ্রহণ করলে, আমরা তিনটি গ্রুপ করতে পারি: ১০০ এর নিচে, ১-১০০ এর মধ্যে, এবং ১০০ এর উপরে।
*   **Boundary Value Analysis (BVA):** ইনপুটের সীমানা বা বর্ডার চেক করা। যেমন: ১-১০০ রেঞ্জের জন্য ০, ১, ২ এবং ৯৯, ১০০, ১০১ চেক করা।
*   **Decision Table Testing:** লজিক্যাল রিলেশন চেক করার জন্য টেবিল ব্যবহার করা।
*   **Error Guessing:** অভিজ্ঞতার ভিত্তিতে সম্ভাব্য ভুলগুলো খুঁজে বের করা।

**ব্যাখ্যা (Bangla):** ব্ল্যাক বক্স টেস্টিং মানে হলো সফটওয়্যারটি বাইরে থেকে কেমন কাজ করছে তা দেখা। এর মূল লক্ষ্য হলো ইউজার যা চাচ্ছে সফটওয়্যার তা দিচ্ছে কিনা তা নিশ্চিত করা।

#### **1(b) Estimate the Cyclomatic complexity of the following flow chart. Verify your answer using Graph matrix theory. (5 Marks)**
**সমাধান:**
প্রদত্ত চিত্র থেকে:
*   Edges (E) = 8 (A, B, C, D, E, F, G, H)
*   Nodes (N) = 6 (1, 2, 3, 4, 5, 6)
*   Connected Components (P) = 1

**Formula 1:** $V(G) = E - N + 2P = 8 - 6 + 2(1) = 4$
**Formula 2:** $V(G) = \text{Predicates} + 1$. চিত্রে ডিসিশন নোড (যেখান থেকে একাধিক পথ বের হয়েছে) হলো ৩টি (Node 1, 2, 4)। সো, $3 + 1 = 4$।
**Graph Matrix:** ম্যাট্রিক্স তৈরি করে $1$ বিয়োগ করে যোগ করলেও ফল ৪ আসবে।

**ব্যাখ্যা (Bangla):** সাইক্লোম্যাটিক কমপ্লেক্সিটি দিয়ে বোঝা যায় একটি প্রোগ্রাম কতটা জটিল। এর মান যত বেশি, প্রোগ্রামটি টেস্ট করা তত কঠিন।

---

### **Question 2**

#### **2(a) Demonstrate characteristics of a good software design with examples. (5 Marks)**
**সমাধান:**
একটি ভালো সফটওয়্যার ডিজাইনের বৈশিষ্ট্য:
1.  **Modularity:** সিস্টেমকে ছোট ছোট মডিউলে ভাগ করা।
2.  **Low Coupling:** মডিউলগুলো একে অপরের ওপর কম নির্ভরশীল হবে।
3.  **High Cohesion:** একটি মডিউল নির্দিষ্ট একটি কাজই ভালোভাবে করবে।
4.  **Maintainability:** সহজে আপডেট করা যাবে।

**ব্যাখ্যা (Bangla):** ভালো ডিজাইন মানে হলো এমন ভাবে কোড সাজানো যাতে ভবিষ্যতে কোনো পরিবর্তন করলে পুরো সিস্টেম ভেঙে না পড়ে।

#### **2(b) Illustrate the different phases or activities of Software Project Management. (5 Marks)**
**সমাধান:**
১. **Planning:** লক্ষ্য নির্ধারণ।
২. **Scheduling:** কাজের সময়সীমা ঠিক করা।
৩. **Risk Management:** সম্ভাব্য ঝুঁকি চিহ্নিত করা।
৪. **Monitoring and Control:** প্রজেক্ট ঠিকঠাক চলছে কিনা তা দেখা।

#### **2(c) Demonstrate the seven principles of risk management in software engineering briefly. (5 Marks)**
**সমাধান:**
১. Global Perspective, ২. Forward-looking view, ৩. Open communication, ৪. Integrated management, ৫. Continuous process, ৬. Shared product vision, ৭. Teamwork.

---

### **Question 3**

#### **3(b) Estimation Problem (Hospital Management System)**
**ডেটা ক্যালকুলেশন (PERT Formula: $E = (S_{opt} + 4S_m + S_{pess}) / 6$):**
1.  **Patient Reg:** $(2500 + 4*3500 + 5500) / 6 = 22000 / 6 = 3666.67$ LOC
2.  **Appt Scheduling:** $(4200 + 4*6300 + 8400) / 6 = 37800 / 6 = 6300$ LOC
3.  **Billing:** $(1800 + 4*2400 + 4800) / 6 = 16200 / 6 = 2700$ LOC

*   **Total LOC** = $3666.67 + 6300 + 2700 = 12666.67$ LOC.
*   **i. Person required per month:** $12666.67 / 4000 \approx 3.17$ PM.
*   **ii. Total cost:** $3.17 \times \$6000 = \$19,020$.
*   **iii. Cost per LOC:** $\$19,020 / 12666.67 \approx \$1.50$.

---

#### **3(c) Critical Path Method (CPM)**
**অ্যাক্টিভিটি নেটওয়ার্ক:**
*   Path 1: A -> F -> G -> H = $7 + 9 + 4 + 3 = 23$ weeks.
*   Path 2: A -> C -> E -> G -> H = $7 + 3 + 4 + 4 + 3 = 21$ weeks.
*   Path 3: A -> D -> H = $7 + 6 + 3 = 16$ weeks.
*   Path 4: B -> D -> H = $5 + 6 + 3 = 14$ weeks.
*   Path 5: B -> E -> G -> H = $5 + 4 + 4 + 3 = 16$ weeks.

**Critical Path:** **A-F-G-H** (যেহেতু এটি দীর্ঘতম পথ)।
**Duration:** 23 weeks.

---

### **সম্পর্কিত গুরুত্বপূর্ণ বিষয় (Topic Details):**
1.  **SDLC Models:** Waterfall, Agile, Scrum (এগুলো থেকে প্রশ্ন আসার সম্ভাবনা বেশি)।
2.  **Software Metrics:** LOC, Function Point (FP) গণনা।
3.  **Testing Types:** White box vs Black box testing.
4.  **Requirement Engineering:** Functional vs Non-functional requirements.

### **অতিরিক্ত প্রশ্ন (Related Questions):**
*   What is the difference between Verification and Validation?
*   Explain the COCOMO model for software cost estimation.
*   Describe the COHESION and COUPLING with diagrams.
*   What is a Gantt Chart and how is it used in project scheduling?





---





### Solve 2


---

## 1(a) Black Box Testing – পদ্ধতি, বর্ণনা + প্রতিটির Example

**Black Box Testing** = সিস্টেমের ভেতরের কোড/লজিক না দেখে শুধু **Input → Output** দেখে টেস্ট করা।

### 1) Equivalence Partitioning (EP)

**আইডিয়া:** ইনপুট ডোমেইনকে কয়েকটা “সমমান গ্রুপ”-এ ভাগ করি, প্রতিটি গ্রুপ থেকে ১টা করে টেস্ট দিলেই ধারণা পাওয়া যায়।
**Example:** বয়স ইনপুট 18–60 valid

* Invalid: `<18`
* Valid: `18–60`
* Invalid: `>60`
  **Test:** 17, 25, 61

### 2) Boundary Value Analysis (BVA)

**আইডিয়া:** ভুল বেশি হয় বাউন্ডারিতে (limit এর কাছাকাছি)।
**Example:** 18–60 valid হলে টেস্ট:

* 17, **18**, 19, 59, **60**, 61

### 3) Decision Table Testing

**আইডিয়া:** একাধিক condition থাকলে সব কম্বিনেশনের জন্য decision table বানিয়ে টেস্ট।
**Example:**

* Condition: (A) User premium? (B) Coupon valid?
* Action: Discount apply?
  কম্বিনেশন: (Y,Y), (Y,N), (N,Y), (N,N) → 4 test

### 4) State Transition Testing

**আইডিয়া:** সিস্টেমের state পরিবর্তন (login/logout/locked) ঠিক আছে কিনা।
**Example:** ভুল পাসওয়ার্ড 3 বার → account locked
টেস্ট: 1st wrong → still active, 3rd wrong → locked, locked অবস্থায় login attempt → denied

### 5) Use Case Testing

**আইডিয়া:** বাস্তব ইউজার ফ্লো অনুযায়ী end-to-end টেস্ট।
**Example:** “Register → Login → Add to cart → Checkout → Payment”

### 6) Error Guessing

**আইডিয়া:** অভিজ্ঞতা থেকে সম্ভাব্য ভুল ধরে টেস্ট।
**Example:** empty input, special char, very long text, invalid date (31/02), negative value ইত্যাদি।

✅ **Related Questions (Practice)**

1. EP আর BVA এর পার্থক্য লিখুন।
2. Decision table দিয়ে “Login + OTP” সিস্টেমের টেস্ট কেস বানান।
3. State transition diagram আঁকুন: Active → Locked → Unlocked.

---

## 1(b) Flow Chart এর Cyclomatic Complexity (Graph Matrix Theory)

প্রশ্নের ফ্লো গ্রাফে **Node = 6** (1..6) এবং **Edge = 8** (A,B,C,D,E,F,G,H) দেখা যাচ্ছে। 

Cyclomatic Complexity:
[
V(G)=E-N+2P
]
যেখানে,

* (E = 8)
* (N = 6)
* (P = 1) (একটা connected component)

[
V(G)=8-6+2(1)=4
]

✅ **Answer:** **Cyclomatic Complexity = 4**
**মানে:** Independent path সংখ্যা 4 → কমপক্ষে 4টা টেস্ট কেস/পাথ কভার করলে basis path coverage পাওয়া যাবে।

✅ **Possible Independent Paths (একটা উদাহরণ)**

1. 6→1→2→4→6
2. 6→1→2→5→6
3. 6→1→2→3→6
4. 6→1→2→4→6 (এ ধরনের লুপ/ভিন্ন কম্বিনেশন ধরে basis set সাজানো হয়)

✅ **Related Questions (Practice)**

1. Cyclomatic complexity বেশি হলে কী সমস্যা হয়?
2. V(G) দিয়ে minimum test case সংখ্যা কীভাবে বের করো?

---

## 2(a) Good Software Design এর বৈশিষ্ট্য + উদাহরণ

### 1) Modularity

ছোট ছোট মডিউলে ভাগ (User, Payment, Inventory)
**Benefit:** change/bug fix সহজ।

### 2) Low Coupling, High Cohesion

* **Low Coupling:** এক মডিউল অন্যটার উপর কম নির্ভরশীল
* **High Cohesion:** এক মডিউলের কাজ একই টাইপের
  **Example:** “Payment module” শুধু payment কাজ করবে, UI কাজ না।

### 3) Maintainability

ভবিষ্যতে আপডেট সহজ।
**Example:** config আলাদা ফাইল, পরিষ্কার structure।

### 4) Reusability

একই component অন্য project এও কাজে লাগবে।
**Example:** OTP sender service reusable।

### 5) Scalability

ইউজার বাড়লে সিস্টেম ভাঙবে না।
**Example:** caching, queue-based email sending।

### 6) Simplicity & Consistency

অপ্রয়োজনীয় complexity কম। naming/structure consistent।

✅ **Related Questions**

1. Cohesion vs Coupling ব্যাখ্যা করুন উদাহরণসহ।
2. “Hospital system” এ modular design কীভাবে করবেন?

---

## 2(b) Software Project Management এর Phases/Activities

1. **Initiation**: objective, feasibility, stakeholder
2. **Planning**: scope, schedule, cost, risk plan, resource plan
3. **Execution**: কাজ ডেভেলপ/ইমপ্লিমেন্ট, টিম ম্যানেজ
4. **Monitoring & Controlling**: progress tracking, KPI, risk handling, change control
5. **Closure**: delivery, documentation, lessons learned

✅ **Related Questions**

1. WBS কী এবং কেন দরকার?
2. Change control না থাকলে কী সমস্যা হয়?

---

## 2(c) Risk Management এর 7 Principles (সংক্ষেপে + বাস্তব উদাহরণ)

1. **Maintain a global perspective** – পুরো সিস্টেম/বিজনেস impact দেখা
2. **Take a forward-looking view** – আগেই সম্ভাব্য ঝুঁকি ধরো
3. **Encourage open communication** – টিমে risk নিয়ে খোলামেলা আলোচনা
4. **Integrate risk management** – প্ল্যানিং/ডেভ/টেস্ট সবখানে risk যুক্ত
5. **Emphasize a continuous process** – একবার না, নিয়মিত
6. **Develop a shared product vision** – সবাই একই লক্ষ্য বুঝবে
7. **Encourage teamwork** – risk response দলগত

✅ উদাহরণ: “Payment gateway down” → contingency: alternate gateway + retry queue.

✅ **Related Questions**

1. Risk exposure কী?
2. Risk mitigation vs contingency plan পার্থক্য লিখুন।

---

## 3(a) Software Cost Estimation Techniques (সংক্ষেপে)

1. **Expert Judgment**: অভিজ্ঞদের অনুমান
2. **Analogous Estimation**: আগের মিল প্রজেক্ট দেখে
3. **Top-down Estimation**: আগে মোট estimate → পরে ভাগ
4. **Bottom-up Estimation**: ছোট টাস্ক estimate যোগ করে মোট
5. **Algorithmic Models (COCOMO)**: ফর্মুলা ভিত্তিক
6. **PERT/Three-point Estimation**: optimistic, most likely, pessimistic

✅ **Related Questions**

1. Top-down বনাম Bottom-up কোনটা ভালো কখন?
2. COCOMO কী ইনপুট নেয়?

---

## 3(b) Hospital Management System – Size, Person-month, Cost, Cost/LOC

প্রশ্নে ৩টা major function আছে এবং প্রতিটায় **3-point estimate** দেয়া:

* Patient registration: (S_{opt}=2500,; S_m=3500,; S_{pess}=5500)
* Appointment scheduling: (4200, 6300, 8400)
* Billing & invoicing: (1800, 2400, 4800) 

### Step-1: PERT Expected Size

[
S_{exp}=\frac{S_{opt}+4S_m+S_{pess}}{6}
]

* Registration:
  [
  \frac{2500+4(3500)+5500}{6}=\frac{22000}{6}=3666.67
  ]
* Appointment:
  [
  \frac{4200+4(6300)+8400}{6}=6300
  ]
* Billing:
  [
  \frac{1800+4(2400)+4800}{6}=2700
  ]

✅ Total LOC:
[
3666.67+6300+2700=12666.67;LOC
]

### Step-2: Person-month

Productivity = 4000 LOC / person-month
[
PM=\frac{12666.67}{4000}=3.1667
]
✅ **Person required per month ≈ 3.17** (মানে প্রায় **3–4 জন** ১ মাস কাজ করলে)

### Step-3: Total cost

Cost = $6000 per person-month
[
Total;Cost=3.1667 \times 6000=19000;USD
]

### Step-4: Cost per LOC

[
\frac{19000}{12666.67}=1.5;USD/LOC
]

✅ **Answers**

1. Person required per month ≈ **3.17**
2. Total cost ≈ **$19,000**
3. Cost per LOC ≈ **$1.50/LOC**

✅ **Related Questions**

1. Productivity 5000 হলে PM কত হত?
2. একই LOC কিন্তু cost rate $8000 হলে cost/LOC কত?

---

## 3(c) CPM: ES/EF/LS/LF + Critical Path

Activities (duration, precedents): 

* A(7) – none
* B(5) – none
* C(3) – A
* D(6) – A,B
* E(4) – B,C
* F(9) – A
* G(4) – E,F
* H(3) – D,G

### Forward Pass (ES/EF)

* A: ES 0 EF 7
* B: ES 0 EF 5
* C (after A): ES 7 EF 10
* D (after A,B): ES max(7,5)=7 EF 13
* E (after B,C): ES max(5,10)=10 EF 14
* F (after A): ES 7 EF 16
* G (after E,F): ES max(14,16)=16 EF 20
* H (after D,G): ES max(13,20)=20 EF 23

✅ Project duration = **23 weeks**

### Backward Pass (LS/LF) + Slack

* H: LF 23 LS 20 (slack 0)
* G: LF 20 LS 16 (slack 0)
* D: LF 20 LS 14 (slack 7)
* F: LF 16 LS 7 (slack 0)
* E: LF 16 LS 12 (slack 2)
* C: LF 12 LS 9 (slack 2)
* A: LF 7 LS 0 (slack 0)
* B: LF 12 LS 7 (slack 7)

✅ **Critical Path (slack = 0):** **A → F → G → H**
Duration = 7 + 9 + 4 + 3 = **23 weeks**

✅ **Related Questions**

1. D এর slack কেন 7 হলো ব্যাখ্যা করুন।
2. যদি F duration 11 হয়, critical path কি বদলাবে?

---



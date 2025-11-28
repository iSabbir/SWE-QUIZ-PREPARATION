# Topic 02: Function Point (FP) Estimation - Mobile Banking Application

A Mobile Banking Application is being developed for a commercial bank. The app supports user login, balance inquiry, fund transfer, transaction history, bill payment, and notifications. It interacts with core banking systems and third-party biller services.

Use the following data to calculate Total Function Points (Unadjusted FP):

| Information Domain Values     | Simple | Average | Complex | Count | FP Count   |
| ----------------------------- | ------ | ------- | ------- | ----- | ---------- |
| Number of inputs              | 4      | 8       | 14      | **8** | 32 = (4×8) |
| Number of outputs             | 5      | 9       | 15      | **7** | 35 = (5×7) |
| Number of inquiries           | 3      | 6       | 11      | **6** | 18 = (3×6) |
| Number of files               | 4      | 9       | 13      | **5** | 20 = (4×5) |
| Number of external interfaces | 3      | 5       | 9       | **4** | 12 = (3×4) |

**Count – Total = ?**  
**Total FP = 32 + 35 + 18 + 20 + 12 = 117**

---

| **Factors (Fi)**                        | **Value** |
| --------------------------------------- | --------- |
| Backup and recovery                     | 5         |
| Data Communication                      | 4         |
| Distributed processing                  | 1         |
| Performance critical                    | 2         |
| Existing operating environment          | 3         |
| On-line data entry                      | 5         |
| Input transaction over multiple screens | 3         |
| Master file updated online              | 1         |
| Information domain values complex       | 4         |
| Internal processing complex             | 2         |
| Code designed for reuse                 | 2         |
| Conversion / installation in design     | 1         |
| Multiple installation                   | 4         |
| Application designed for change         | 3         |
| **Sum(Fi)**                             | **40**    |

# Topic 02: Function Point (FP) Estimation - Online Library Management System

A medium-sized Online Library System is being developed. It will manage book borrowing, searching, digital member profiles, notifications, and librarian dashboards.

Use the following data to calculate Total Function Points (Unadjusted FP):

| Information Domain Values     | Simple | Average | Complex | Count | FP Count   |
| ----------------------------- | ------ | ------- | ------- | ----- | ---------- |
| Number of inputs              | 3      | 8       | 14      | **8** | 24 = (3×8) |
| Number of outputs             | 4      | 7       | 15      | **7** | 28 = (4×7) |
| Number of inquiries           | 2      | 6       | 10      | **6** | 12 = (2×6) |
| Number of files               | 4      | 10      | 12      | **5** | 40 = (4×5) |
| Number of external interfaces | 2      | 5       | 8       | **3** | 6 = (2×3)  |

**Count – Total = ?**  
**Total FP = 24 + 28 + 12 + 40 + 6 = 110**

---

| **Factors (Fi)**                        | **Value** |
| --------------------------------------- | --------- |
| Backup and recovery                     | 3         |
| Data Communication                      | 2         |
| Distributed processing                  | 1         |
| Performance critical                    | 4         |
| Existing operating environment          | 3         |
| On-line data entry                      | 4         |
| Input transaction over multiple screens | 2         |
| Master file updated online              | 4         |
| Information domain values complex       | 2         |
| Internal processing complex             | 3         |
| Code designed for reuse                 | 1         |
| Conversion / installation in design     | 2         |
| Multiple installation                   | 5         |
| Application designed for change         | 3         |
| **Sum(Fi)**                             | **39**    |

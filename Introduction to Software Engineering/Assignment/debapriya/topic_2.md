# Topic 02: Function Point (FP) Estimation - Online Hotel Reservation System

An Online Hotel Reservation System allows customers to search rooms, check availability, book rooms, cancel bookings, and view booking history. The system also interacts with external payment gateways and hotel management dashboards.

Use the following data to calculate Total Function Points (Unadjusted FP):

| Information Domain Values     | Simple | Average | Complex | Count | FP Count   |
| ----------------------------- | ------ | ------- | ------- | ----- | ---------- |
| Number of inputs              | 3      | 6       | 12      | **9** | 27 = (3×9) |
| Number of outputs             | 4      | 7       | 13      | **6** | 24 = (4×6) |
| Number of inquiries           | 3      | 5       | 9       | **5** | 15 = (3×5) |
| Number of files               | 5      | 10      | 15      | **4** | 20 = (5×4) |
| Number of external interfaces | 2      | 4       | 8       | **3** | 6  = (2×3) |

**Count – Total = ?**  
**Total FP = 27 + 24 + 15 + 20 + 6 = 92**

---

| **Factors (Fi)**                        | **Value** |
| --------------------------------------- | --------- |
| Backup and recovery                     | 2         |
| Data Communication                      | 3         |
| Distributed processing                  | 2         |
| Performance critical                    | 5         |
| Existing operating environment          | 4         |
| On-line data entry                      | 3         |
| Input transaction over multiple screens | 4         |
| Master file updated online              | 2         |
| Information domain values complex       | 3         |
| Internal processing complex             | 4         |
| Code designed for reuse                 | 1         |
| Conversion / installation in design     | 3         |
| Multiple installation                   | 2         |
| Application designed for change         | 4         |
| **Sum(Fi)**                             | **42**    |

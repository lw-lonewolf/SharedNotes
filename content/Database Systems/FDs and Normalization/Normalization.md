Normalization is the process of **removing redundancy** and **avoiding anomalies** in relational databases. It divides a table into **smaller, well-structured** tables.

### **Why Normalize?**

- **Removes redundancy** (avoids duplicate data).
- **Eliminates anomalies** (insertion, update, deletion).
- **Increases efficiency** in queries.

### **Normalization Forms (Normal Forms - NFs)**

#### **🔹 1NF (First Normal Form) – Atomicity**

- No **repeating groups** or multivalued attributes.
- All columns must have **atomic values** (indivisible).
- Each row must have a **unique identifier** (Primary Key).

**Example (Not in 1NF - multivalued attributes):**

|Student_ID|Student_Name|Courses|
|---|---|---|
|101|Alice|CS, Math|
|102|Bob|IT|

**1NF Fix:**

|Student_ID|Student_Name|Course|
|---|---|---|
|101|Alice|CS|
|101|Alice|Math|
|102|Bob|IT|

---

#### **🔹 2NF (Second Normal Form) – No Partial Dependency**

- Must be in **1NF**.
- No **partial dependency** (i.e., a non-key attribute cannot depend on part of a composite key).

**Example (Not in 2NF - Partial Dependency):**

|Student_ID|Course|Instructor|Instructor_Age|
|---|---|---|---|
|101|CS|Smith|45|
|102|Math|John|50|

Here, **Instructor_Age** depends only on **Instructor**, not on **(Student_ID, Course)**.

**2NF Fix - Split into two tables:**  
**Student_Course Table:**

|Student_ID|Course|Instructor|
|---|---|---|
|101|CS|Smith|
|102|Math|John|

**Instructor Table:**

|Instructor|Instructor_Age|
|---|---|
|Smith|45|
|John|50|

---

#### **🔹 3NF (Third Normal Form) – No Transitive Dependency**

- Must be in **2NF**.
- No **transitive dependencies** (i.e., a non-key attribute cannot depend on another non-key attribute).

**Example (Not in 3NF - Transitive Dependency):**

|Employee_ID|Employee_Name|Department_ID|Department_Name|
|---|---|---|---|
|201|Alice|10|HR|
|202|Bob|20|IT|

Here, **Department_Name** depends on **Department_ID**, not on **Employee_ID**.

**3NF Fix - Split into two tables:**  
**Employee Table:**

|Employee_ID|Employee_Name|Department_ID|
|---|---|---|
|201|Alice|10|
|202|Bob|20|

**Department Table:**

|Department_ID|Department_Name|
|---|---|
|10|HR|
|20|IT|

---

#### **🔹 BCNF (Boyce-Codd Normal Form) – No More Anomalies**

- Stronger than **3NF**.
- No **overlapping candidate keys** (only one candidate key should determine attributes).

**Example (Not in BCNF - Violation of Candidate Key Rule):**

|Student_ID|Course|Instructor|
|---|---|---|
|101|CS|Smith|
|102|Math|John|

Here, **(Student_ID, Course)** is the primary key, but **Instructor** also determines **Course**, violating BCNF.

**BCNF Fix:**  
**Student_Course Table:**

|Student_ID|Course|
|---|---|
|101|CS|
|102|Math|

**Instructor Table:**

|Course|Instructor|
|---|---|
|CS|Smith|
|Math|John|

---

### **🔹 4NF (Fourth Normal Form) – No Multivalued Dependency**

- Must be in **BCNF**.
- Removes **multivalued dependencies** (when an attribute depends on a key but independently from other attributes).

**Example:**

| Student_ID | Course | Hobby    |
| ---------- | ------ | -------- |
| 101        | CS     | Chess    |
| 101        | CS     | Painting |
| 101        | Math   | Chess    |

Here, **Student_ID -> Hobby** and **Student_ID -> Course**, but these should be separate.
r
**4NF Fix - Split into two tables:**  
**Student_Course Table:**

|Student_ID|Course|
|---|---|
|101|CS|
|101|Math|

**Student_Hobby Table:**

|Student_ID|Hobby|
|---|---|
|101|Chess|
|101|Painting|

---

### **🔹 5NF (Fifth Normal Form) – No Join Dependency**

- Must be in **4NF**.
- Removes join dependencies (where decomposed tables can be joined back without data loss).
- Rarely needed in practical databases.
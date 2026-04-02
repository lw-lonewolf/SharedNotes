A **functional dependency** (FD) is a constraint that expresses a relationship between attributes in a relation (table). It helps determine **normal forms** in database normalization.

### Definition
If A->B, it means that for a given value of A, there is only one unique value of B.
	A is called the *Determinant*.
	B is called the *Dependent*. 

### **Example:**

| Student_ID | Student_Name | Major |
| ---------- | ------------ | ----- |
| 101        | Alice        | CS    |
| 102        | Bob          | IT    |
| 103        | Alice        | CS    |

Here, **Student_ID → Student_Name** means that knowing the **Student_ID** uniquely determines the **Student_Name** (but the reverse is not necessarily true).

### **Types of Functional Dependencies:**

1. **Trivial Dependency**: If **A → B**, but B is a subset of A. (E.g., **{A, B} → B** is trivial).
2. **Non-Trivial Dependency**: If **A → B**, and B is NOT a subset of A.
3. **Completely Non-Trivial Dependency**: If **A → B**, and A & B have no common attributes.
4. **Multivalued Dependency (MVD)**: If **A →→ B**, then for one A value, multiple B values exist independently of other attributes.
5. **Transitive Dependency**: If **A → B** and **B → C**, then **A → C** is a transitive dependency (bad for 3NF).

See [[Normalization]] for how to deal with these.
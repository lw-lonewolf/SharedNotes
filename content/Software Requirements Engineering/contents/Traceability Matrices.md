-### 1. **Requirements Linkage Traceability Matrix (Sparse Example)**

| Requirement ID | Design Spec | Code Module   | Test Case |
| -------------- | ----------- | ------------- | --------- |
| 1.1            | D1          | AuthModule    | TC1       |
| 1.1.1          | D2          | ResetModule   | TC2       |
| 1.2.1          | D3          | EncryptModule | TC3       |
| 2.1            | D4          | ReportModule  | TC4       |
| 3.1.1          | D5          | SearchModule  | TC5       |
### 2. **Requirements Source Traceability Matrix (Sparse Example)**

| Requirement ID | Source Document | Regulatory Body | Stakeholder        |
| -------------- | --------------- | --------------- | ------------------ |
| 1.1            | BRD-01          | -               | Product Owner      |
| 1.1.1          | -               | ISO27001        | Compliance Officer |
| 1.2            | BRD-02          | -               | End User           |
| 2.1            | -               | GDPR            | Legal Team         |
| 3.1            | -               | -               | Developer Team     |

- **Explanation**: This matrix links requirements to their sources, such as documents (BRD = Business Requirements Document), regulatory bodies (ISO, GDPR), and stakeholders. The empty cells represent areas without a link for a specific requirement.

### 3. **Requirements Stakeholder Traceability Matrix (Sparse Example)**

| Requirement ID | 1.1 | 1.1.1 | 1.2 | Developer Team |
| -------------- | --- | ----- | --- | -------------- |
| 1.1            | R   | U     | -   | -              |
| 1.1.1          | R   | -     | -   | -              |
| 1.2            | -   | R     | U   | -              |
| 2.1            | -   | -     | R   | -              |
| 3.1.1          | -   | -     | -   | R              |

- **Explanation**: This matrix connects requirements to specific stakeholders, showing who is responsible (R) or has an interest (U - User) in each requirement.

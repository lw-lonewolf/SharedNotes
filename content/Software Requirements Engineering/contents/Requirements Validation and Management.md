* Review: *a formal/informal assessment of requirements to ensure correctness and completeness*
* Inspection: *a structured process where a team examines the requirements in detail to identify defects*
* Walk-through *a step by step presentation of requirements, typically led by author, to gather feedback*
* Checklists *a predefined list of criteria used to verify that all necessary aspects of the requirements are covered.*
* Reading *a technique where stakeholders independently read the requirements to detect issues*
* Interviews *direct discussions with the stakeholders to clarify, validate or gather additional requirements*
* Prototyping *creating a simplified model of the system to validate requirements through user feedback*
* Simulation *using models to mimic the system's behavior, helping validate feasibility and functionality of requirements*

# Traceability: 
Traceability ensures each requirement is tracked through out the development process, both across system levels and within each stage of development. 

#### Horizontal Traceability: 
* *Links requirements across various components or artifacts in the same development stage or level of development (e.g. from system requirements to sub-system requirements)*
* **Example**: In a software system, a requirement for user authentication might have horizontal traceability across related design documents, test cases, and source code components. If the requirement specifies two-factor authentication, horizontal traceability ensures that:

- The design document for the user interface reflects this,
- The code includes modules for password and token-based authentication,
- Test cases are created to verify both password and token validation.
#### Vertical Traceability: 
* *Tracks requirements through different levels of abstraction in the development phase, from high-level requirements to detailed implementation or testing*
* **Example:** For the same user auth feature, vertical traceability would ensure alignment: 
	* From a high-level business requirement (`The system must ensure secure user auth`)
	* To a functional requirement (`Implement 2FA using password and auth code`)
	* To a design sepcification (`UI flow`, `backend architecture`)
	* To the implementation (`code`)
	* To test cases and test results.

### Conclusion (TLDR)
**Horizontal traceability** connects related elements within the same stage, while **vertical traceability** connects different levels of development, from high-level requirements to detailed implementations.
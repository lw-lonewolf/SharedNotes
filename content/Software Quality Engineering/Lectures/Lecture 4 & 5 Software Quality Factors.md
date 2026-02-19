## The McCall's Quality Factor Model
This model classifies all software requirements into 11 software quality factors. These 11 factors are classified into three groups. 

* *Product Operation Factors (5):* Correctness, Reliability, Efficiency, Integrity, Usability
* *Product Revision Factors (3):* Maintainability, Flexibility, Testability
* *Product Transition Factors (3):*  Portability, Usability, Interoperability
### Product Operation Factors 
Mostly details with day to day operations.
#### Correctness 
The sub-dimensions of correctness are as follows: 
* Output
* Accuracy
* Completeness
* Uptodateness
* Availability
* Standards

### Product Revision Factors
Mostly deals with changes.
#### Maintenance & Evolution
Maintenance has the following different types
* Corrective Maintenance
* Adaptive Maintenance
* Perfective Maintenance
* Additive Maintenance

### Product Transition Factors
Mostly deals with the software's interactions with it's environment.
#### Portability
It should be capable of working in different environments. If it works in Windows, it shall work in Mac OS/Linux as well. If it works on MS Edge it should work on Chrome etc. as well 
#### Re-usability
It has two different forms: 
* with (past) {use existing stuff}
* for (future) {make with the intention to reuse in the future}
#### Interoperability
A lot of software needs to interact or "interoperate" with another software and *these software must be listed under (the interoperability section of the SRS) of the software.* Compatibility in every day usage may refer to **EITHER** portability or interoperability.

## Quality Factor Models and their Number of Quality Factors

| QF Model          | Year | Number of Quality Factors |
| ----------------- | ---- | ------------------------- |
| McCalls Model     | 1977 | 11                        |
| Evans & Marciniak | 1987 | 12                        |
| Deutsch & WIllis  | 1988 | 15                        |
Added Quality Factors: 
* Verifiability -> both 2nd and 3rd proposed
* Safety
* Manageability
* Survivability -> very similar to Reliability
* Expandability -> very similar to Flexibility -> both 2nd and 3rd proposed

#### Verifiability
Important for some very critical applications. Basically means should be verifiable through formal languages.
#### Survivability

#### Safety
These requirements are there to prevent *hazards*.
#### Manageability
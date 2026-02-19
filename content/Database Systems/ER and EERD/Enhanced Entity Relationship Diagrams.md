### Difference between an ERD and a EERD 
![[Pasted image 20250422010906.png]]
Inheritance etc are the main difference between EERD. 

### Inheritance
#### Specialization (Top Down)
A parent exists (Employee) which has children (secretary, technician, engineer). 
#### Generalization (Bottom Up)
First children classes are built and then based on characteristics they are made part of a general class, this is generalization. e.g. truck and car are made part of a vehicle class. 

## Disjoint vs Overlapping
Disjoint: The sub-classes are disjoint e.g. one employee can be at one point a secretary, technician or an engineer not more than one.

Overlapping: Person(parent) -> women(child) -> driver(child) -> engineer(child). Basically a case where one parent entity may belong to more than one child class.

![[Pasted image 20250422011529.png]]
(When there is just one sub class)

![[Pasted image 20250422011552.png]]

(The double line shows total participation. an employee WILL be either salaried or will have a pay scale.)
### Category/Union Type 
![[Pasted image 20250422014023.png]]
A union type means that AT LEAST ONE parent must exist (there may be more than one).
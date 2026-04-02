*Rectangles* -> Entities 
*Diamonds* -> Relationships
## Attributes 
**Simple**: Ellipse
**Key**: Ellipse with underline
**Derived**: Dashed Ellipse 
**Multi-valued**: More than one phone e.g.
**Composite**: One attribute divides into further children attributes. The children are stored in the db not the main parent attribute.
**Complex**: If two things are combined (e.g. complex and also composite for example. its a complex attribute).
**Descriptive**: An attribute attached to the relationship instead of an entity. 

## Relationship 
### Constraints 
#### Cardinality
##### 1 to 1 Cardinality 
ONE Employee manages ONE department. 
##### 1 to Many Cardinality 
MANY Employees work for ONE Department
##### Many to Many 
MANY Employees work on MANY projects. (one employee works on many projects, one project is worked on by many employees)

>[!warning] Why use M:N instead of M;M
>Not necessary for both sides to have EQUAL numbers, e.g. 10 employees may work on 3 projects

>[!info] Relation Between Two Entities 
>Two entities are never attached directly, they must have a [diamond] in between

## Recursive Relationship 
![[Entity Relationship Diagrams 2025-04-22 00.51.49.excalidraw]]
It is compulsory to mention roles (supervisor, supervisee) in a recursive relationship.

## Strong Entity vs Weak Entity 
If an entity can define itself properly its a strong entity. 
On the other hand an entity with a weak relationship its a weak entity. *It is denoted by a double rectangle*.
![[Entity Relationship Diagrams 2025-04-22 00.56.54.excalidraw]]

## Participation
If some entity is COMPLETELY involved in a relationship we use a double line for it. We denote this be a **double line**. (e.g. a department must be managed by one employee). *This is a complete or total participation*

On the other hand an employee may or may not managed a department so this is a partial participation.*Single line*

### Degree of a Relationship
* Unary
* Binary
* Ternary
Ternary is broken down normally. 

![[Pasted image 20250422010522.png]]

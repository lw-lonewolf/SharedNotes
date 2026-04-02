A functional dependency (FD) has the form (X -> Y) where X and Y are sets of attributes in a relation R 

X -> Y means that whenever two tuples in R agree on all the atrributes in X, they must also agree on all attributes in Y 


| X   | Y            | Z                  |
| --- | ------------ | ------------------ |
| a   | b            | c                  |
| a   | b(Must be b) | ?(can be anything) |
| ..  | ..           | ..                 |
For any two tuples t1 and t2 in any relation instance r(R): 
If t1[X] = t2[X], then t1[Y] = t2[Y]

* We can say in other words, that *X* **functionally determines** Y 
* X -> Y in R specifies a constraint on all instances r(R)

##### Example: 
StudentGrade(SID, name, email, CID, grade)
* SID -> name, email 
* email -> CID 
* SID, CID -> grade
(Not a good design)


##### Another Example: 
Address (street_address, city, state, zip)

* street_address, city, state → zip
* zip → city, state
* zip, state → zip?
	* This is a trivial FD
	* Trivial FD: LHS ⊇ RHS
* zip -> state, zip?
	* This is non-trivial but not completely non-trivial
	* Completely non-trivial FD: LHS $\cap$ RHS = $\phi$

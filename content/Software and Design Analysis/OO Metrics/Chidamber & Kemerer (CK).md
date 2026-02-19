#### Weighted Methods per Class 
$$WMC = \sum_{i=1}^{n} C_{i}$$
Sum of complexities of n methods, assuming all methods have complexity =1 for our cases so WMC = number of operations 
#### Depth of Inheritance Tree (DIT)
same as D from LK. 
#### Number of Children (NOC) 
Count of immediate children (**NOT GRANDCHILDREN**)
#### Coupling between Objects (CBO)
 -> check SDA notes for this 
#### Response for a Class (RFC) 
Count number of operations and number of remote operations called by those operations (number of external functions called)
#### Lack of Cohesion of Methods (LCOM) 
* Calculated for every Class
* Every class has its own LCOM values
* most complicated

$I = \{i_{1}, i_{2}, i_{3},\dots ,i_{m}\}$   //set of all instance of class's non static variables 
$M =\{M_{1}, M_{2}, M_{3}, \dots M_{n}\}$ //set of methods of a class

$$M_{1}\to I_{1}, \quad M_{2}\to I_{2} \quad M_{n} \to I_{n}$$
$P = \{(I_{v}, I_{s}) | I_{v}\cap I_{s} = \emptyset\}$ 
$Q = \{(I_{v}, I_{s} | I_{v} \cap I_{s} \neq \emptyset)\}$// set of all pairs with common 

###### Total Useful Pairs 
The total pairs can be found as $\frac{n(n-1)}{2} = |P|+|Q|$



$$LCOM = |P| -|Q| \quad \land \quad  |P| >|Q|$$
Else if $|P|<|Q|$ then $LCOM = 0$



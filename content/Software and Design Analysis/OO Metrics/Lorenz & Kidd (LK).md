
***This is LK Model for OO Metrics. It focuses more on the size for project management***
#### Number of Scenario Scripts (NSS) 
Count the number of use cases or ovals 
#### Number of Sub-System (NSUS)
Count the number of packages 
#### Number of Key Classes (NKC)
Use the *ACD* to count the number of classes 
#### Number of Supporting Classes (NSC)
* Persistent Classes (student, faculty in flex are key classes) and classes like 'registration controller' are supporting classes 
#### Average Supporting Classes Per Key Class (ASC)
$$ASC = \frac{NSC}{NKC}$$
(Tells how much an ACD expands to a DCD)
#### Class Size 
$$\text{Class Size} = NO + NA$$

where $NO$ is number of operations and $NA$ is the number of attributes
#### Depth of a Class (d) 
How deep a class is. At top depth = 0, then increases downwards. 
#### Number of Operations added by subclasses (NOA)
(self explanatory)
#### Number of Operations Overridden (NOO) 
(self explanatory)
#### Specialization Index (SI) 
$$SI = \frac{NOO*D}{NO}$$

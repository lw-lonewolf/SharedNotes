Anomalies -> any abnormal behavior that the system shows. 

What to do when integrity is violated. Several actions can be taken.
(FOR UPDATE)
-> Cancel the option that causes this. 
-> Perform but inform the user
-> Trigger additional updates so violation is corrected. 
-> Follow the user defined violation handling. 

(FOR INSERT)
-> *Domain Constraint* (changed datatype)
-> *Key Constraint* (key already exists)
-> *Referential Integrity* (foreign key references a primary key value that does not exist)
-> *Entity Integrity* -> (Check slides)
#### Armstrong's Inference Rules
1) IR1. ***Reflexive***: 
	 If $Y \subseteq X$, then $X\to Y$
2) IR2. ***Augmentation***: 
	 If $X\to Y$, then $XZ\to YZ$
3) IR3. ***Transitive***:
	 If $X\to Y$ and $Y\to Z$, then $X\to Z$
* ***Decomposition***
	If $X\to YZ$, then $X\to Y$ and $X\to Z$
* ***Union*** 
	If $X\to Y$ and $X\to Z$, then $X\to YZ$
* ***Pseudotransitivity***
  If $X\to Y$ and WY->Z, then WX->Z

**Closure** of a set F of FDs is the set $F^{+}$ of all FDs that can be inferred from F 

**Closure** of a set of attributes X with respect to F is the set $X^+$  of all attributes that are functionally determined by X

$X^+$ can be calculated by repeatedly applying IR1, IR2, IR3 using the FDs in F 

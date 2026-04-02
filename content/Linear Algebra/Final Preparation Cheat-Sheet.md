### Chapter 1: Systems of Linear Equations 
`Gaussian Elimination` -> Reduce Matrix to Row Echelon Form  
`Gauss-Jordan Elimination` -> Reduce Matrix to Reduced Row Echelon Form 
`Pivot Rows` -> Rows containing the leading non-zero element, used in the reduction process to make zeros in the other lines above and below 
`Pivot Columns` -> Rows containing the leading non-zero element, used in the reduction process to make zeros in the other lines above and below 
##### Proof: 
*Prove that if $AB$ and $BA$ are both defined then $AB$ and $BA$ are square matrices 

Let order of $A$ = $(m \times n)$ and B = $(p \times q)$
Then $AB$ exists only if $n = p$ and BA exists only if $m = q$
That is $B$ = $(n \times m)$, which means $AB = (m \times m )$ and $BA = (n \times n)$
##### Proof: 
*Prove that B = (n x m) if A(BA) is defined if A = (m x n)*
Let B = $(p \times q)$
order of BA = $(p \times q)(m \times n)$ -> $(q  = m)$
order of A(BA) = $(m \times n)( p \times q)$
			   = $(m \times n)(p \times n)$
	this multiplication will only  be possible if $p = n$
Hence B = $(p \times q)$ = $(n \times m)$

##### Direct Method for Answer (Example 8) 
If problem is in the form: 
$$\begin{aligned}
u = ax + by \\ v = cx + dy
\end{aligned}$$
Then a direct solution is 
$$
\begin{aligned}
x = \frac{du - bv}{ad - bc}\\\\
y = \frac{av - cu}{ad -bc}
\end{aligned}
$$ 
##### Proof: 
*Show that if A is invertible and AB = AC then B = C*
As $A^{-1}$ exists 
Multiplying both sides with $A^{-1}$ 
$A^{-1}AB = A^{-1}AC \to IB = IC \to B = C$ , as $AA^{-1} = I$

*Show that if A, B, and A+B are invertible matrices with
the same size, then A(A^−1 + B^−1)B(A+ B)−1 = I*
$A(A^{-1} + B^{-1})B(A+B)^{-1} = I$
$(BAA^{-1} + BB^{-1}A^{-1})(A+B)^{-1} = I$
$(B + A)(A+B)^{-1} = I$
$I = I$

#### Inversion Algorithm 
Write matrix in augmented form with an identity matrix of the same order, make identity on the original side. the right side will be the inverse of original matrix 
$$
\begin{array}{cc}
a &b | 1 &0\\
c &d | 0 &1
\end{array}
$$
#### Matrices and Their Inverses in Form Of Elementary Matrices 

Take the matrix and reduce it to reduced row echelon form (REEF). Perform only Elementary operations and note each elementary matrix. e.g if performing $R_{1} + 2R_{2}$ on a $2 \times 2$ matrix. The elementary matrix for this operation would be: 
$$\begin{bmatrix}
1  & 2 \\
0  & 1
\end{bmatrix}$$
This is acquired by performing the same operation on $I_{2}$
$$\begin{bmatrix}
   1 + (2 \cdot 0) & 0 + (2 \cdot 1)  \\
0  & 1
\end{bmatrix}$$
Then the formula for Matrix in form of Elementary Matrices is given as: 

$\dots E_{4}E_{3}E_{2}E_{1}A = I$
so that 
$$A ={E_{1}}^{-1} {E_{2}}^{-1}{E_{3}}^{-1}\dots I$$
and 
$$A^{-1} = \dots E_{4}E_{3}E_{2}E_{1}$$
This answer is not unique and may depend on what the applied elementary functions were.

### Chapter 2: Determinants 

>[!NOTE] Theorem  2.3.3
>A square matrix is invertible only if det(A) != 0

>[!NOTE] Theorem 2.3.4
>If $A$ and $B$ are square matrices of the same size, then 
>det(AB) = det(A)det(B)

> [!NOTE] Theorem 2.3.5
> If $A$ is invertible then, 
>  $\det(A^{-1}) = \frac{1}{\det(A)}$

##### Adjoint of a Matrix above 2x2 order

-> Find all the Cofactors. Make an array $X$ of these cofactors 
$$
X = \begin{bmatrix}
C_{11} & C_{12}  & C_{13} \\
C_{21} & C_{22}  & C_{23} \\
C_{31} & C_{32}  & C_{33} \\
\end{bmatrix}
$$
Now, 
$$\text{Adj. of A} = X^t = \begin{bmatrix}
C_{11}  & C_{21}  & C_{31} \\
C_{12}  & C_{22}  & C_{32} \\
C_{13}  & C_{23}  & C_{33} \\
\end{bmatrix} $$
##### Equivalent Theorem

If $A$ is an $n \times n$ matrix, then the following statements are equivalent.
(a) $A$ is invertible.
(b) $Ax = 0$ has only the trivial solution.
(c) The reduced row echelon form of $A$ is $In$.
(d) $A$ can be expressed as a product of elementary matrices.
(e) $Ax = B$ is consistent for every $n \times 1$ matrix $B$.
(f) $Ax = B$ has exactly one solution for every $n \times 1$ matrix $B$.
(g) $\det A \neq 0$.

## Chapter 3: Euclidean Vector Spaces 
The components of a vector in 3-space that has initial point P1$(x_{1}, y_{1}, z_{1})$ and terminal point P2$(x_{2}, y_{2}, z_{2})$ are given by 
$$\vec{P_{1}P_{2}} = (x_{2} - x_{1}, y_{2}- y_{1}, z_{2}-z_{1})$$
Refer to [[3.1 Euclidean Vector Space|Lecture Notes for 3.1]] for detailed info on certain topics.
##### Equality: 
Two vectors are equal only if their components are equal to each other 
$$\begin{aligned}
\vec{v} = (a, b, c, d) \\ 
\vec{w} = {1, -4, 2, 7} 
\end{aligned}$$
then $\vec{v} = \vec{w}$ if $a = 1, b = -4, c = 2, d= 7$
##### A Linear Combination 
If $W$ is a vector in $R^n$ then $w$ is said to be a *linear combination* of the vectors $\vec{v_{1}}, \vec{v_{2}}, \vec{v_{3}} \dots$ if it can be expressed as 
$$\vec{W} = k_{1}\vec{v_{1}} + k_{2}\vec{v_{2}} + k_{3}\vec{v_{3}} + \dots$$
where $k_{1},k_{2}, k_{3}, \dots$ are *coefficients* of the linear combination. 

We can also write a vector $\vec{v} = (a,b,c)$ in;
 $$\text{Row-Vector Form} = \vec{v} = \begin{bmatrix}
a & b & c
\end{bmatrix}$$
and
$$
\text{Column-Vector Form} = \vec{v} = \begin{bmatrix}
a \\
b \\
c \\
\end{bmatrix}
$$
##### Norm of a Vector 

$$||\vec{v}|| = \sqrt{v_{1}^2 + v_{2}^2}$$
##### Unit Vector
$$ \vec{ u} = \frac{1}{||\vec{v}||} \vec{v}$$
Obtaining a unit vector from a vector is known as normalizing it.

#### Distance in $R^n$
$$d = ||\vec{P_{1}P_{2}}|| = \sqrt{ (x_{2}-x_{1})^2 + (y_{2}-y_{1})^2 }$$
More generally, 
$$d(\vec{u}, \vec{v}) = ||\vec{u} - \vec{v}|| = \sqrt{ (u_{1}-v_{1})^2 + (u_{2}-v_{2})^2+\dots+(u_{n}-v_{n})^2 }$$
Distance between a point $P_{0}(x_{0}, y_{0})$ and a line $ax+by+c = 0$
$$D = \frac{ax_{0} + by_{0}+c}{\sqrt{ a^2 + b^2 }}$$
For a plane: 
$$D = \frac{ax_{0} + by_{0}+cz_{0} + d}{\sqrt{ a^2 + b^2 +c^2}}$$
For distance between two planes, take arbitrary point on one line by setting $y = 0 , z = 0$, then use above formula. 

##### Dot Product (Euclidean Inner Product)
$$\vec{u} \cdot \vec{v} = ||\vec{u}||\cdot||\vec{v}||\cdot \cos \theta$$
$\theta < 90$ if $\vec{u} \cdot \vec{v} > 0$
$\theta > 90$ if $\vec{u} \cdot \vec{v} < 0$
$\theta = 90$ if $\vec{u} \cdot \vec{v} = 0$

In component form: 
$\vec{u} \cdot \vec{v} = u_{1}v_{1} + u_{2}v_{2} + u_{3}v_{3}$ 

##### Cauchy-Schwarz Inequality and Angles in $R^n$
$$\theta  = \cos^{-1}{\frac{\vec{u}\cdot \vec{v}}{||\vec{u}||\cdot ||\vec{v}||}}$$
provided that $\frac{\vec{u}\cdot \vec{v}}{||\vec{u}||\cdot ||\vec{v}||}$ is in the range [-1, 1] (inclusive)
Basically, 

>[!important] Cauchy Schwarz Inequality
>If $u$ = $u_{1}, u_{2}, u_{3}, \dots, u_{n}$ and $v = (v_{1}, v_{2}, v_{3}, \dots v_{n}$ are vectors in $R^n$ then
>$$|\vec{u}\cdot \vec{v}| \leq ||u|| \cdot ||v||$$

##### Triangle Inequality 
If $u$ and $v$ and $w$ are vectors in $R^{n}$, then: 
(a) $||\vec{u} + \vec{v} || \leq ||\vec{u}|| + ||\vec{v}||$
(b) $d(\vec{u}, \vec{v}) \leq d(\vec{u}, \vec{w}) + d(\vec{w}, \vec{v})$
![[triangle ineq pt1.png]]
![[triangle ineq pt2.png]]
##### Parallelogram Equations for Vectors
If $u$ and $v$ are vectors in $R^{n}$, then
$$||\vec{u}+\vec{v}||^2 + ||\vec{u}-\vec{v}||^2 = 2(||\vec{u}||^2 + ||\vec{v}||^2)$$

$$A\vec{u}\cdot v = \vec{u}\cdot A^T\vec{v}$$
or
$$\vec{u}\cdot A\vec{v} = A^T\vec{u}\cdot\vec{v}$$

##### Orthogonal Vectors
Two vectors are known to be orthogonal if their dot product is equal to zero.
$$\vec{u} \cdot \vec{v} = 0$$
##### Lines and Planes Determined by Points and Normals

A *normal* is *nonzero* and *orthogonal* to the line or plane in the question. Line through Point $P_{0}(x_{0}, y_{0})$ that has normal $n$ = $(a,b)$. Then these are represented as 
$$\vec{n}\cdot \vec{P_{0}P} = 0$$
where $P$ is an arbitrary point $P(x, y)$
Hence Equation can be written as: 
$$a(x-x_{0}) + b(y-y_{0}) = 0$$
$$a(x-x_{0}) + b(y-y_{0}) + c(z-z_{0})= 0$$
These are called point-normal equations of the line and the plane. Here $n(a,b)$ and $n(a,b,c)$ are the *normals* or *orthogonal* vectors to the line on which both these points lie.

Now, homogeneous equations in two or three unknowns can be written as 
$$\vec{n} \cdot \vec{x} = 0$$
where $n$ is the vector of coefficients and $x$ is the vector of unknowns.

##### Projection Formulae: 
vector component of $\vec{u}$ along $\vec{a}$
$$\text{proj}_{a}\vec{u} = \frac{\vec{u}\cdot \vec{a}}{||a||^2}a$$
Vector Component of $u$ orthogonal to $a$
$$\vec{u} - \text{proj}_{a} \vec{u} = \vec{u} -\frac{\vec{u}\cdot \vec{a}}{||a||^2}a$$
>[!info] Pythagoras Theorem in $R^n$
>If $u$ and $v$ are orthogonal vectors in $R^{n}$ with the Euclidean inner product, then
>$$||\vec{(u+v)}||^2 = ||\vec{u}||^2 + ||\vec{v}||^2$$

##### Parametric Equations of Lines and Planes 
$$x = x_{0} + t\vec{v}$$
and 
$$x = x_{0} + t_{1}\vec{v_{1}} + t_{2}\vec{v_{2}}$$

##### Line Through Two Points in $R^n$
$x = x_{0} + t(x_{1}- x_{0})$
or 
$x = (1-t)x_{0} + tx_{1}$
This is the *two-point vector equations* of a line in $R^n$
(Also the *line segment between two points $x_0$ $x_1$*)


##### Cross Product of Two Vectors 
If $u$ = $(u_{1}, u_{2}, u_{3})$ and $v$ = $(v_{1}, v_{2}, v_{3})$ are vectors in 3-space, then the cross product $u \times v$ is defined by 
$$u \times v = (u_{2} v_{2} - u_{3}v_{2}, v_{3}v_{1}- v_{1}v_{3}, v_{1}v_{2} - u_{2}v_{1})$$
Geometrically, 
$$||u \times v|| = ||u||||v||\sin \theta$$
#####  / Relations between Dot/Cross Product 
-> $u \cdot (u \times v) = 0$ [u x v is orthogonal to u]
-> $v. (u\times v) = 0$ [u x v is orthogonal to v]
-> $||u \times v|| ^2 = ||u||^2||v||^2 - (u \times v)^2$ [Lagrange's Identity]
-> $u \times (v \times w) = (u \cdot w)v - (u \cdot v)w$ [vector triple product]
-> $(u \times v) \times w) = (u \cdot w)v - (v \cdot w)u$ [vector triple product]c x

##### Area of a Parallelogram

$$A = (base)(altitude) = ||u||||v||\sin \theta = ||u \times v||$$
##### Area of a Triangle 
Half of the area of a Parallelogram
$$\frac{1}{2} ||u\times v||$$
##### Scalar Triple Product / Volume of Parallelepiped
$$\vec{u} \cdot (\vec{v} \times \vec{w})$$
is called the *scalar triple product* of $u$, $v$, $w$

$$\vec{u} \cdot (\vec{v} \times \vec{w}) = \det(\begin{bmatrix}
u_{1} & u_{2} & u_{3} \\
v_{1} & v_{2} & v_{3} \\
w_{1} &  w_{2} & w_{3}  \\
\end{bmatrix})$$
$V$ = $|\vec{u} \cdot (\vec{v} \times \vec{w})|$

$|u \cdot (v \times w)| = 0$ if and only if the vectors $u$ and $v$ and $w$ lie in the same plane. 

##### Area of a Tetrahedron
$\frac{1}{6} |\vec{u} \cdot (\vec{v} \times \vec{w})|$


## Chapter 2: General Vector Spaces

##### Vector Space Axioms 
If all of these axioms are satisfied then it is a vector space. 

> [!important] Vector Space Axioms
> 1) If $u$ and $v$ are objects in $V$ then $u + v$ is in $V$
> 2) $u + v = v + u$
> 3) $u + (v+w) = (u+v) + w$
> 4) There exists a zero vector $\vec{0}$ such that $\vec{0} + u = u+\vec{0} = u$
> 5) $\forall u \in V \text{ there exists } -u \in V$ called negative of $u$ such that $u + (-u) = (-u)+u = \vec{0}$
> 6) If $k$ is any scalar and $u$ is any object in $V$, then $ku$ is in $V$.
> 7) $k(\vec{u} + \vec{v} = k\vec{u} + k\vec{v})$
> 8) $(k+m)\vec{u} = k\vec{u} + m \vec{u}$
> 9) $k(m\vec{u}) = (km)(\vec{u})$
> 10) $1\vec{u} = \vec{u}$

##### Subspaces
A subset $W$ of a vector space $V$ is called a *subspace* of $V$ if $W$ is itself a vector space under the addition and scalar multiplication defined on $V$.
In order to prove that a $W$ is a subspace of $V$ we must prove: 
a) If $\vec{u}$ and $\vec{v}$ are vectors in $W$, then $u+v$ is in $W$ 
b) If $k$ is a scalar and $\vec{u}$ is a vector in $W$ then $k\vec{u}$ is in $W$

###### Zero Subspace
If V is any vector space and if W = $\{0\}$ is the subset of $V$ that consists of the zero vector only, then W is closed under addition and scalar multiplication. We call W the *zero subspace* of $V$

>[!info] Theorem 4.2.2
>If $W_{1},W_{2},\dots,W_{r}$ are subspaces of $V$ then the intersection of these subspaces is also a subspace of V.

##### Spanning Sets
If $w$ is in a vector space $V$, then $w$ is said to be a **linear combination** of the vectors $v1, v2, \dots, v_{r}$ in $V$ if $w$ can be written as: 
$$w = k_{1}v_{1} + k_{2}v_{2} + \dots k_{r}v_{r}$$
>[!warning] A Spanning Set
>If $S = \{w_{1}, w_{2}, \dots, w_{r}\}$ is a nonempty set of vectors in a vector space $V$, then: 
>a) The set $W$ of all possible linear combinations of the vector in $S$ is a subspace of $V$. 
>b) The set $W$ in part (a) is the "smallest" subspace of $V$ that contains all of the vectors in $S$ in the sense that any other subspace that contains those vectors contains $W$

The subspace $W$ is called the subspace of $V$ *spanned* by $S$. The vectors $w_{1}, w_{2}, \dots , w_{n}$ in $S$ are said to *span* $W$.

> In order for $w$ to be a linear combination of $u$ and $v$. The following must be true: 
>   $w = k_{1}u+k_{2}v$

> [!Important] How to check if vectors span a vector space 
> Express equation in terms of its components: 
>  $$b = k_{1}v_{1} + k_{2}v_{2} + k_{3}v_{3}$$
>  or 
>   $$(b_{1}, b_{2}, b_{3}) = k_{1}(1,1,2) + k_{2}(1, 0, 1) + k_{3}(2,1,3)$$
> for matrix, check determinant. If its zero than it does not span. (or to be more clear check if its consistent or inconsistent)

##### Linear Independence

If $S$ is a set of two or more vectors in a vector space $V$, then $S$ is said to be a linearly independent set if no vector in $S$ can be expressed as a linear combination of the other.
>[!IMPORTANT] How to Check
>$S$ is linearly independent only and only if $k_{1}, k_{2}, \dots, k_{r}$ that satisfy this equation:
> $$k_{1}v_{1} + k_{2}v_{2} + \dots + k_{r}v_{r} = \vec{0}$$
> are $k_{1} = 0, k_{2}=0, \dots, k_{r} = 0$

Easy way for square matrices -> take determinant -> if det(A) = 0 which means that it is linearly dependent, otherwise solve system.

>[!IMPORTANT] Theorem 4.4.2
>a) A set with finitely many vectors that contains 0 is linearly dependent. 
>b) A set with exactly two vectors is linearly independent if and only if neither vector is a scalar multiple of the other. 

>[!IMPORTANT] Theorem 4.4.3
>Let $S = \{v_{1}, v_{2}, \dots, v_{r}\}$ be a set of vectors in $R^n$. If $r>n$ then $S$ is linearly dependent
>(BASICALLY IF THE NUMBER OF VECTORS IS GREATER THEN THE DIMENSION OF R, ITS A LINEARLY DEPENDENT SET)

##### Basis for a Vector
If $S$ is $\{v_{1}, v_{2}, \dots, v_{n}\}$ is a set of vectors in a finite-dimensional vector space $V$, then S is called a *basis* for V if: 
a) $S$ spans $V$. 
b) $S$ is linearly independent.

---
(ATP I WAS DONE WITH LA. WENT TO GIVE PAPER :sad:)

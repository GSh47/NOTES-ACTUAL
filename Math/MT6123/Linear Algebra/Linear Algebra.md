Jumping to subspaces

Let $n$ be a natural number let $P_{n}(F)$ consist of all polynomial in $P(F)$ having degree $\leq n$ since zero polynomial has degree $-1$, it is in $P_{n}(F)$ 

if $, F(x)+G(x)\in$ 
Let $c$ be an element $deg(cf(x))\leq n$ then so $cP_{n}(F)\in F$ ?? 

Let $c(\mathbb{R})$ define all single valued functions in $\mathbb{R}$ then 
for any $f,g\in FF(R,\mathbb{R})$ be any two functions in $\mathbb{R}$ then $f(x)+g(x)\in FF(\mathbb{R})$ note that $f(t)=0\forall t\in \mathbb{R}$ 
we know that constant functions are continuous, so $c(R)$ is closed under additiion and scalar multiplication ? hence $c(\mathbb{R})$ is a subspace of $\mathbb{R},\mathbb{R}$ 

Example : set of all $n\times n$ diagonal matrices are a subspace of $M_{n\times n}(F)$ is the set of all $n\times n$ matrices with entries from the field $F$. 

1. We know that 0 matrix is a diagonal matrix 
2. if A and B are digonal matrix, then their sum $A+B$ is also a diagonal matrix 
3. for any scalar element $c\in F$ then $cA$ is a diagonal matrix

trace of $n\times n$ matrix $M$ denoted by $tr(M)$ is the sum of the diagonal entries of $n$. i.e set of all $n\times n$ matrices having trace zero is subspace of $M_{n\times n}(F)$ 

1. Trace of zero matrix is zero, 
2. if trace of $A$ is zero and trace of B is zero, then trace of $A+B=tr(A)+tr(B)=0$ 
3. trace(cA)$=ctr(A)$

Let $c(\mathbb{R})$ be the vectorspace of all real valued continuous functions defined over $\mathbb{R}$ then the set $W$ of solutions of the differential equation $$a_{2} \frac{d^{2}y}{dx^{2}}+a_{1} \frac{dy}{dx}+a_{0}y=0$$ where $a_{1},a_{2},a_{0}\in \mathbb{R}$ is a subspace of $V$. 
If $y_{1}$ an $y_{2}$ are solutions, then wkt $c_{1}y_{1}+c_{2}y_{2}$ is a solution of the differential equation. 

The set of all matrices in $M_{n\times n} (R)$ having non negative entries is not a subspace. (if $c=-k$ then it's a negative matrix, thus not closed under scalar multiplication ) 

#theorem  Any intersection of subspaces is a subspace. 
Every straight line passing through origin is a subspace of $\mathbb{R}2$ over $\mathbb{R}$ because equation of a straight line passing through origin and with slope $m$  is given by $y=mx$. ie $w=\{ y=mx :x\in \mathbb{R} \}$. 

1. $(0,0)$ is an element of $w$ as they both pass through origin. 
2. If $c\in\mathbb{R}$ and $(x,y)\in w$, then $c(x,y)\in w$ are 

---
hint: The union of two subspaces can always be a subspace if one of them lies within the other

- Sum of two subspaces is a subspace
# Linear Combination
Let  $V$ be a vectorspace over field $F$, Let $S$ be a non empty subset of $V$ a vector $v\in V$ is called a linear  combination of vector of $S$ if there exists a finite number of vectors $u_{1},u_{2},\dots\in S$ and $a_{1},a_{2},\dots a_{n}\in F$ such that $v=a_{1}u_{1}+a_{2}u_{2}+\dots+a_{n}u_{n}$. We say that $v$ is  a linear combination of $u_{1},u_{2},\dots$ and $a_{1},a_{2},a_{3}\dots$

**verify whether vector $(-2,0,3)$ is a vector under $(1,3,0)\&(2,4,-1)$**
$$
\begin{aligned}
(-2,0,3)=&a(1,3,0)+b(2,4,-1) \quad a,b\in\mathbb{R}\\
=&(a+2b,3a+4b,-b)\\\implies& b=-3,a=4
\end{aligned}
$$
We must solve by jordan gauss eliminination too !
**Verify whether the polynomial $x^{3}-3x+5$ can be expressed as a linear combination of $x^{3}+2x^{2}-x+1$ and $x^{3}+3x^{2}-1$**
The vectorspace is $P_{3}(\mathbb{R})$ and this corresponds to a matrix problem of the sort 
$(1,0,-3,5)=a(1,2,-1,1)+b(1,3,0,-1) \quad a,b\in \mathbb{R}$ solved to get $3,-2$

# Linear Span 

Let $S$ be a non empty subset of a  vectorspace $V$ over $F$ the span of $S$ denoted by $span(S)$ is hte set consisting of all linear combination of vectors in $S$ 
WKT $\mathbb{R}_{3}\to \mathbb{R}$ is vector space, given a subspace $S=\{ (1,0,0),(0,1,0) \}\in\mathbb{R}_{3}$
$$
\begin{aligned}
span(S)=&\{a(1,0,0)+b(0,1,0):a,b\in\mathbb{R}  \}\\
=&\{(a,0,0)+(0,b,0):a,b\in\mathbb{R}  \}\\
=&\{(a,b,0):a,b\in\mathbb{R}  \}
\end{aligned}
$$
which is the $xy$ plane passing through origin.  which is a subspace of $\mathbb{R^3}$ 

#theorem **The span of any subset $S$ of a vector space $V$ is given to be a subspace of V,moreover any subspace of $V$ that contains $S$ must also contain span of $S$ span of any subspace is a subspace**

If $S=\varnothing$ 
then $span(S)=\{ 0 \}$ which is a trivial subspace of any vectorspace.

If $S\neq\varnothing$ 
Then $\exists u\in S$ thus,
1. $0\cdot u=0$
2. $x,y\in span(S)$, then $\exists u_{1},u_{2},\dots\&v_{1},v_{2},\dots \in V$
$\ni x=a_{1}u_{1}+a_{2}u_{2}+\dots +a_{n}u_{n},\quad y=b_{1}v_{1}+b_{2}v_{2}+\dots+b_{n}v_{n}$ 
 $\implies x+y=(a_{1}u_{1}+b_{1}v_{1})+(a_{2}u_{2}+b_{2}v_{2})+\dots(a_{n}u_{n}+b_{n}v_{n})$ as $x+y$ itself is a linear combination of vectors from $S$, we say $x+y\in span(S)$ 
 1. if $x=a_{1}v_{2}+a_{2}v_{2}\dots$ $cx=c(a_{1}v_{1}+a_{2}v_{2}+\dots)=(ca_{1})v_{1}+(ca_{2})v_{2}+\dots$
which is a linear combination this $\in span(S)$ 


Let $x,y\in span(S)$ Then there exists vectors $u_{1},u_{2},\dots,u_{m}$ and $v_{1},v_{2},\dots v_{n}$ such that $x=a_{1}u_{1}+a_{2}u_{2}+\dots+a_{m}u_{m}$ and 
$y=b_{1}v_{1}+b_{2}v_{2}+\dots+b_{n}v_{n}$ 
for scalars $a_{1},a_{2},\dots,b_{1},b_{2},\dots.\in F$ 
thus $x+y\in span(S)$ 

Span $S$ is a subspace of $V$ over $F$, 

TO prove any subspace of $V$ that contains $S$ must also contain span of $S$. 
Consider subspace $W$ and $w\in span(S)$ and $w=c_{1}w_{1}+cw_{2}\dots+c_{nw_{n}}$ for $w_{1},w_{2},\dots,w_{n}\in S$ and $c_{1},c_{2},\dots,c_{n}\in F$ 
now that $S\subseteq W$ implies $w_{1},w_{2},\dots,w_{n}\in W$ 
Thus every vector in span $S\in W$ thus, 
$Span(S)\in W$ 

#theorem A subset $S$ of vectorspace $V$ generates (or spans) $V$ if $span (S)=V$ in this case we also say that vectors of $S'dash'V$ ?  
![[Pasted image 20250115084244.png]]

Determine whether $\begin{pmatrix} 1 &2\\-3&4 \end{pmatrix}$ is in the span of $S=\{\begin{pmatrix}1&0\\-1&0\end{pmatrix},\begin{pmatrix}0&1\\0&1\end{pmatrix},\begin{pmatrix}1&1\\0&0\end{pmatrix} \}$

Show if $M_{1}=\begin{pmatrix}1&0\\0&0\end{pmatrix},M_{2}=\begin{pmatrix}0&0\\0&1\end{pmatrix},M_{3}=\begin{pmatrix}1&0\\0&1\end{pmatrix}$ forms set of all symmetric matrices 

Show that span $\{ x^{2}+x+1,x \}=span\{ x^{2}+1,x \}$ in $P(F)$ 

For what value of $k$  will vector will $(1,k,5)$ be a linear combination of $(1,-3,2)$ and $(2,-1,1)$ : gives $(a+2b=1,-3a-b=k,2a-b=5$ so... -7 ?

# Linear dependence and independence

A subset $S$ of a vector space $V$ is called linearly dependent if there exists a finite number of distinct vectors $u_{1},u_{2},\dots u_{n}$ in $S$ and scalars $a_{1},a_{2},\dots a_{n}$ in $F$ not all zero such that their linear combination is zero. In this case we also say that the vectors of $S$ are linearly dependent. 

Note: the zero vetor has a trivial representation as linear combination of $u_{1},u_{2},\dots,u_{n}$ given by $0=u_{1}+u_{2}+\dots+u_{n}$ 

A set is linearly dependent if there exists a non trivial representation of zero. as a linear combination of vectors in teh set. Consequently any subset of vector space that contins the zero vector is linearly dependent. Since $0=1\times 0$ is a non trivial representation of zero as a linear combination of vectors in the set

Know that if $S=\{ 0,V_{1} \}$ then $0=1\cdot0 +0 \cdot V$ 

**Consider the set $\{ (1,3,-4,2),(2,2,-4,0),(1,-3,2,-4),(-1,0,1,0) \}$ show that $S$ is linearly dependent and then express one of the vectors in $S$ as a linear combination of vectors in $S$**
As in reap, represent all vectors as a linear combination

$$
\begin{aligned}
a(1,3,-4,2)+\\b(2,2,-4,0)+\\c(1,-3,2,-4)+\\d(-1,0,1,0)\\ \\ =(1+2b+c-d,\\3a+2b+2c,\\-4a-4b+2c+d,\\ 2a-4c)
\end{aligned}
$$


**Find if lin dep** $span\{ x^{3}-x,2x^{3}+4,-2x^{3}+3x^{2}+2x+6 \}$ 
$$
\begin{pmatrix}
1 & 0 & -1 \\
0 & 3 & 0 \\
-1 & 2 & 0 \\
0 & 6 & 4
\end{pmatrix}
$$
we see that rank is 3 and dim is 3 

![[matrix.png]]

# Theorem of linear dependence ?
#theorem  Let $U$ and $V$ be distinct vectors in a vectorspace, show that $\{ u,v \}$ is linearly independent iff $u$ or $v$ is  a multiple of the other. 
Let $u,v:u\neq v\in V$ if $u$ and $v$ are linearly dependent, then there exists scalars (not all zero) such that $c_{1}u+c_{2}v=0$  

claim : $c_{1}u+c_{2}v=0$ and $c_{1}\neq 0\neq c_{2}$ 
if $c_{1}\neq 0$ 
$$
\begin{aligned}
c_{1}u+c_{2}v=0\\
c_{1}u=-c_{2}v\\u=\left( -\frac{c_{2}}{c_{1}} \right)v
\end{aligned}
$$

if $c_{2}\neq 0$ 
$$
\begin{aligned}
c_{1}u+c_{2}v=0\\
c_{1}u=-c_{2}v\\u=\left( -\frac{c_{2}}{c_{1}} \right)v
\end{aligned}
$$
then the  general case:
$$
\begin{aligned}
c_{2}v=-c_{1}v\\v=\left( -\frac{c_{1}}{c_{2}} \right)u
\end{aligned}
$$


Conversely, If $u$ and $v$ are multiples of each other, 
case 1:
 
$$
\begin{aligned}
u=c_{1}v\quad c_{1}\in F\\
1\cdot u-c_{1}v=0\\1\cdot u+(-c_{1})v=0
\end{aligned}
$$
hence $\{ u,v \}$ are linearly dependent. 
similarly, case 2 : $v=c_{2}u$ 
gives $1\cdot v+(-c_{2}) \cdot u=0$ thus $\{ u,v \}$ is linearly dependent. 

# Linear Inependence
A subset $S$ of a vectorspacce that is not linearly dependent is called Linearly Dependent. We say that vectors of $S$ aare linearly independent
- A set consisting of a single non zero vector is linearly independent. example : $\{ \varnothing \}$ 
- However the set of zero vectors is not independent. 
- If $u$ is linearly dependent then $au=0$ for some non zero scalar $a$ 
- Any subspace with zero vector is dependent 
- A set is linearly independent if the only representation of zero as linear combinations of it's vectors are trivial representations. 
- A set with finite elements $v_{1},v_{2}\dots v_{n}$ is linearly independent iff $c_{1}v_{1}+c_{2}v_{2}+\dots+c_{nv_{n}}=0$ can happen only if $c_{1}=c_{2}=\dots=0$ 

Example 1: $S=\{(1,0,0,-1),(0,1,0,-1),(0,0,1,-1),(0,0,0,1)  \}$ 
$$
\begin{aligned}
c_{1}(1,0,0,-1)+c_{2}(0,1,0,-1)+c_{3}(0,0,1,-1)+c_{4}(0,0,0,1)=0\\c_{1}=c_{2}=c_{3}=0\\\implies c_{4}=0
\end{aligned}
$$

**For $k=0,1,2,\dots,n$ Let $P_{k}(x)=x^k+x^{k+1}+\dots+x^k$Then the set $\{ P_{0}(x),P_{1}(x),\dots,P_{n}(x) \}$ is linearly independent subset of $P_{n}(F)$**

To prove that the set $\{ P_{0}(x), P_{1}(x), \dots, P_{n}(x) \}$ is linearly independent in the vector space $P_{n}(F)$ (the space of polynomials of degree at most $n$ over a field $F$), we need to show that the only solution to the equation:

$$
c_0 P_0(x) + c_1 P_1(x) + \dots + c_n P_n(x) = 0
$$

is $c_0 = c_1 = \dots = c_n = 0$, where $c_0, c_1, \dots, c_n$ are scalars in $F$.

---

### Step 1: Write out the polynomials $P_k(x)$
For $k = 0, 1, 2, \dots, n$, the polynomial $P_k(x)$ is defined as:

$$
P_k(x) = x^k + x^{k+1} + \dots + x^k.
$$

However, this definition seems redundant because $x^k + x^{k+1} + \dots + x^k$ simplifies to $x^k$ (since all terms are the same). This suggests there might be a typo in the problem statement. Instead, let's assume the correct definition is:

$$
P_k(x) = x^k + x^{k+1} + \dots + x^n,
$$

which is a polynomial of degree $n$ for each $k$. This interpretation makes sense in the context of the problem.

---

### Step 2: Write the linear combination
Consider the linear combination:

$$
c_0 P_0(x) + c_1 P_1(x) + \dots + c_n P_n(x) = 0.
$$

Substitute the definition of $P_k(x)$:

$$
c_0 (x^0 + x^1 + \dots + x^n) + c_1 (x^1 + x^2 + \dots + x^n) + \dots + c_n (x^n) = 0.
$$

---

### Step 3: Collect like terms
Rewrite the equation by collecting terms with the same power of $x$:

$$
c_0 x^0 + (c_0 + c_1) x^1 + (c_0 + c_1 + c_2) x^2 + \dots + (c_0 + c_1 + \dots + c_n) x^n = 0.
$$

For this equation to hold for all $x$, the coefficient of each power of $x$ must be zero. This gives us the system of equations:

$$
\begin{cases}
c_0 = 0, \\
c_0 + c_1 = 0, \\
c_0 + c_1 + c_2 = 0, \\
\vdots \\
c_0 + c_1 + \dots + c_n = 0.
\end{cases}
$$

---

### Step 4: Solve the system of equations
From the first equation, $c_0 = 0$. Substituting $c_0 = 0$ into the second equation gives $c_1 = 0$. Substituting $c_0 = c_1 = 0$ into the third equation gives $c_2 = 0$. Continuing this process, we find:

$$
c_0 = c_1 = c_2 = \dots = c_n = 0.
$$

---

### Step 5: Conclude linear independence
Since the only solution to the equation $c_0 P_0(x) + c_1 P_1(x) + \dots + c_n P_n(x) = 0$ is $c_0 = c_1 = \dots = c_n = 0$, the set $\{ P_0(x), P_1(x), \dots, P_n(x) \}$ is linearly independent in $P_n(F)$. 

---

### Final Answer:
The set $\{ P_0(x), P_1(x), \dots, P_n(x) \}$ is linearly independent in $P_n(F)$.

#theorem **let $V$ be a vectorspace and let $S_{1}\subset S_{2}\subset V$. If $S_{1}$ is linearly dependent, then $S_{2}$ is dependent.** 
Assume $S_{1}$ is dependent, then there exists finite number of vectors $v_{1},v_{2},\dots,v_{n}\in S_{1}$ and constants $a_{1},a_{2},\dots a_{n}\in \mathbb{F}$ such that $a_{1}v_{1}+a_{2}v_{2}+\dots+a_{n}v_{n}=0$  $\mathbb{1}$
but $v_{1},v_{2},\dots,v_{n}\in S_{2}$ from $\mathbb{1}$ we can say $S_{2}$ is linearly dependendent. 

#theorem **Let $V$ be a vectorspace and let $S_{1}\subset S_{2}\subset V$ If $S_{2}$ is  linearly independent then $S_{1}$ is linearly independent.** 

Let $u_{1},u_{2},\dots u_{n}\in S_{2}$ and $a_{1},a_{2},\dots\in \mathbb{F}$. If $a_{1}u_{1}+a_{2}u_{2}+\dots+a_{n}u_{n}=0$ implies that $a_{1}=a_{2}=\dots=a_{n}=0$ 
Since $S_{1}\subset S_{2}$ the above condition is saatisfied by elements of $S_{1}$ as well. thus $S_{1}$ is linearly independent

#theorem **Let $S$ be a linearly independent subset of a vectorspace $V$ and let $v\in V$ and $v\notin S$ then $S\cup \{ v \}$ is linearly dependent iff $V\in Span(S)$**

let $v\in V$ and $v\notin S$, assume that $S\cup \{ v \}$ is linearly dependent.. 
Let $u_{1},u_{2},\dots u_{n}\in S\cup v$ we have $a_{1}u_{1}+a_{2}u_{2}+\dots+a_{n}u_{n}=0$ for $a_{1},a_{2},\dots a_{n}\in\mathbb{F}$ for not all zero, 

Since $S$ is linearly independent,  $\exists u_{i}=v$ for some $i\in[1,n]$ 
here $a_{1}\neq0$, or else then $a_{2}u_{2}+a_{3}u_{3}+\dots+a_{n}u_{n}=0$ which is a contradiction as $S$ is linearly dependent.  
So, $a_{1}^{-1}(a_{1}v+a_{2}u_{2}+\dots+a_{n}u_{n})=0$ then we have $(a_{1}^{-1}a_{1})v=-(a_{1}^{-1}a_{2}u_{2}+a_{1}^{-1}a_{3}u_{3}+\dots+ a_{1}^{-1}a_{n}u_{n})$ 
Thus, $v\in span(S)$
as $u_{1},u_{2},\dots u_{n}\in S$ 
- [ ] copy note here
note that $v\neq v_{i}\forall v=1,\dots m$ since $v \notin S$ and   so coeff of $v$ in this linear combination is non zero, so the set $\{ v,v_{1},v_{2},\dots v_{m} \}$ is linearly deendent
note suppose that $S$ is any linearly dependent set containing 2 or more vectors, some vector $v\in S$ can be written as a linear combination of other vector in $S$ and the subset obtained by removing $v$ from $S$ has the same span as $S$
If no proper subset of $S$ generates span of $S$ then $S$ must be linearly independent. 

# Basis and Dimension 

> A basis $B$ for vectorspace $V$ is a linealry independent subset of $V$ that generates $V$ if $B$ is a basis for $V$ then we also say that the vectors of $B$ form a basis for $V$ 

note that $\varnothing$ the nullset is not a vectorspace is linearly independent, and it's span is the zero vector :$span(\varnothing)=\{ \vec{0} \}$ 


#theorem Let $V$ be a vectorspace and $B=\{ v_{1},v_{2},\dots \}$ be a subset of $V$. $B$ is a subset of $V$ iff each $v\in V$ can e expressed as a linear combination of the vectors of $B$ 

#proof Let $v\in V$ then $v\in span(V)$ $v=a_{1}v_{1}+a_{2}v_{2}+a_{3}v_{3}+\dots a_{n}v_{n}$ for some $a\in \mathbb{F}$ and $v_{n}\in V$ 
Assume $v=b_{1}v_{1}+b_{2}v_{2}+\dots+b_{n}v_{n}$ 
by subtracting the two equations,$$
0=(a_{1}-b_{1})v_{1}+(a_{2}-b_{2})v_{2}+\dots+(a_{n}-b_{n})v_{n}
$$since B is linearly independent, $a_{1}=b_{1},a_{2}=b_{2},\dots,a_{n}=b_{n}$ hence a unique combination. 

Conversely find the proof. 

#note  if $\{ v_{1},v_{2},\dots v_{n} \}$ is a basis of $V$ over $\mathbb{F}$ then for every vector $v\in V$ there exists unique scalars $c_{1},c_{2},\dots,c_{n}\in \mathbb{F}:v=c_{1}v_{1}+c_{2}v_{2}+\dots c_{n}v_{n}$ 

#theorem **The mapping $v\mapsto(c_{1},c_{2},\dots c_{n})$ is an isomorphism from V to $\mathbb{F}$** 
**The vectorspace $V$ is generated by finite set $S$ when some subset of $S$ is a basis for $V$ hence $V$ has a finite basis.** 
let $V$ be a vectorspace over $\mathbb{F}$ 
Let $S$ contained in $V$ such that $span (S)=V$. 

If $S=\varnothing$:
Then $V=span(\varnothing)$ we know that $\varnothing$ is linearly independent subset of $\{ 0 \}$ thus $\varnothing$ is a basis for $V$ 

If $S=\{ 0 \}$ : Then $\varnothing$ is a subset of $S$ which is a basis for $V$ 

Now assume that $S$ is a nonempty subset of $V$ $S\neq \{ 0 \}$, i.e $S$ contains a non zero vector say $u_{1}$. Then $\{ u_{1} \}$ is a linearly independent subset of $V$ if span of $\{ u_{1} \}=V$ implies it is a basis. 
Otherwise $span(u_{1})\neq V$ i.e $span(u_{1})\subset V$ then we can choose a vector $u_{2}\in S$ such that $u_{2} \notin span{(u_{1})}$ 

If $v\in S$ then $S \subset span(u_{1})$ then we can choose $u_{2 such that 

If $\{ u_{1},u_{2} \}$ forms a basis for $V$ then we are done otherwise choose a vector $u_{3}\in S$ such that $u_{1},u_{2},u_{3}$ is linearly independent. Continuing like this since $S$ is a finite set we must eventually reach a stage at ehich $B=\{ u_{1},u_{2},\dots u_{k} \}$ is a linearly independent subset of $S$ adjoined to $B$ any vector from $S$ not in $B$ produces a linearly dependent set. I.e $B$ is a maximal linealry independent subset of $S$. 
Now if $v\in S$ 
If $v\in B$, then $v\in span(B)$ 
If $v \notin B$, then $B\cup \{ v \}$ is linearly dependent. 
So, $v\in span(B)$, thus $S \subset span(B)\implies Span(S) \subset span(B)$ 
i.e, $V \subset span(B)$ 
But $span(B)\subset V$ 
from above we  can say $span(B)=V$ hence $B$ forms the basis and thus $V$ has a finite basis. 
*A finite spanning set for $V$ can be reduced to a basis for $V$* 

# Replacement theorem 
Let $V$ be a vector space that is generated by a set $G$ containing exactly $n$ vectors, and let $L$ be a linearly independent subset of $V$ containing exactly $m$ vectors. Then $m < n$ and there exists a subset $H$ of $G$ containing exactly $n-m$ vectors such that $L\cup H$ generates $V$. 

#corollary let $V$ be a vectorspace having a finite basis then every basis for $V$ contains the same number of vectors 
#proof  let $B$ be a finite basis of $V$ with a finite cardinality of $B$, $|B|=n$. 
If $B'$ be any other basis for V. If $B'$ contains more than n vectors, then we can select a subset S of $B'$ containing  $n +1$ vectors. 
then S is linearly independent and $span(B)=V$ by replacement theorem. 
![[ex1.png]]

# Finite dimensional vectorspaces
 has a basis consisting of a finite number of vectors. The unique number of vectors in each basis for $V$ is called the dimension of $V$ is given as $dim(V)$ . Else is infinite dimensional 

The vectorspace $\{ 0 \}$ has dimension : 0. 
The vectorspace $\mathbb{F^n}$ has dimension $n$
The vectorspace $\mathbb{P_{n}}$ has dimension $n+1$ 
Dimension of $\mathbb{C}$ over $\mathbb{C}$ is $1$ because the scalars can be complex too 
Dimension of $\mathbb{C}$ over $\mathbb{R}$ is $2$ because the scalars can only be real. $\{ 1,i \}$
Dimension of vectorspace depends on the field of scalars 

If vectorspace $V$ is finite dimensional $dim(V)=m$ then a linealry independent subset of $V$ cannot contain more than $2$ vectors i.e every linearly independent subset of $V$ is finite. So a vectorspace which has infinite linearly subset has infinite dimensions eg:  $\{ 1,x,x^{2},\dots \}$ is a basis for $\mathbb{P(F)}$ 

**Corollary** #corollary  Let $V$ be a vectorspace with dim $m$ 

- Any finite generating set for $V$ contains atleast $n$ vectors and a generating set for $V$
  that contains exactly $n$ vectors is a basis for $V$ 
- Any linearly subset of $V$ that contains exactly $n$ vectors is a basis for $V$ 
- Every linearly independent subset of $V$ can be extended to a basis in $V$
- 
#proof   
(a) Let G be a finite generating set for V. By Theorem 1.9 some subset H of G is a basis for V. Corollary 1 implies that H contains exactly n vectors. Since a subset of G contains n vectors, G must contain at least n vectors. Moreover, if G contains exactly n vectors, then we must have H = G, so that G is a basis for V. 
(b) Let L be a linearly independent subset of V containing exactly n vectors. It follows from the replacement theorem that there is a subset H of 
ft containing n — n = 0 vectors such that L U H generates V. Thus H = 0, and L generates V. Since L is also linearly independent, L is a basis for V. 
(c) If L is a linearly independent subset of V containing $n$ vectors, then the replacement theorem asserts that there is a subset H of B containing 
exactly $n-m$ vectors such that LU H generates V. Now L U H contains at most n vectors; therefore (a) implies that L U H contains exactly n vectors and that L U H is a basis for V. 

# Linear Transformations 
Let $V$ and $W$ be vectorspaces over $\mathbb{F}$. A function from $T:V\to W$ is a transformation if $\forall x,y\in V,c\in\mathbb{F}$ we have 
$$
\begin{matrix}
T(x+y)=T(x)+T(y) \\
T(cx)=cT(x)
\end{matrix}
$$
If $T:V\to W$ is linear, then
1. $T(0)=0$
2. $T(x\pm y)=T(x)\pm T(y)$
3. $T(cx+y)=cT(x)+T(y)$ 
and conversely $\forall x,y\in V, c\in \mathbb{F}$ 

#proof 
$$
\begin{matrix}
T(0)=T(0+0) \\
\implies T(0)=T(0)+T(0) \\
T(0)-T(0)=T(0) \\
0=T(0)
\end{matrix} 
$$
$$
\begin{aligned}
T(x-y)=T(x)+T(-y)\\
=T(x)+(-1)T(y)\\=T(x)-T(y)
\end{aligned}
$$
$$
\begin{aligned}
T(cx+y)=T(cx)+T(y)\\=cT(x)+T(y)
\end{aligned}
$$

**Prove that $T:\mathbb{R}^{2}\to \mathbb{R}$ by $T(a_{1},a_{2})=(2a_{1}+a_{2},a_{1})$  over $\mathbb{R}$ Show that $T$ is a linear transformation** 

It is sufficient to prove that $T(kx+y)=kT(x)+T(y)$ thingy 
Let $x=(x_{1},x_{2}),y=(y_{1},y_{2})$ be any two vectors from some vectorspace $V$ 
$$
\begin{aligned}
T(Kx+y)=&KT(x)+T(y)\\
T(K(x_{1},x_{2})+(y_{1},y_{2}))=&KT(x_{1},x_{2})+T(y_{1},y_{2})\\
T(Kx_{1}+y_{1},Kx_{2}+y_{2})=&K(2x_{1}+x_{2},x_{1})+(2y_{1}+y_{2},y_{1})\\
T()
\end{aligned}
$$
and prove LHS = RHS 



[[Rank Nullity Theorem]] 
# Rank nullity theorem (Dimension theorem)
Let $V,W$ be vectorspaces, and let $T:V\to W$ be linear, Let the nullspace $N(T)$ and rank $R(T)$ be finite dimensional then the dimensions are mentioned as Nullity and Rank 

If $V$ is finite dimensional, then Rank(T)+Nullity(T)=dim(V) 
#proof 
Suppose that dimension of $V=n$, and $dim(N(T))=k$ and $\{ v_{1},v_{2},\dots,v_{k} \}$ is a basis for $N(T)$ 
So, we know that - if $W$ is a subspace of finite dimensional vectorspace $V$ then any basis for W can be extended to a basis for $V$ (Replacement Theorem)
Hence, we may extend $\{ v_{1},v_{2},\dots,v_{k} \}$ to a basis for $V$, say $\beta=\{ v_{1},v_{2},\dots,v_{n} \}$ we claim that $S=\{ T(V_{k+1}),T(V_{k+2}),\dots T(V_{n}) \}$ is a basis for $R(T)$ i.e the rangespace of $T$ 


First we prove that $S$ generate $R(T)$ : 
Let $w\in R(T)$ or $w=T(V)$ for some $v\in V$, 
$w=T(c_{1}v_{1}+c_{2}v_{2}+\dots+c_{k}v_{k}+\dots+c_{n}v_{n})$ where $c_{i}\in F,v_{i}\in \beta$ the basis for $V$ 
since $T$ is linear, $w=c_{1}T(v_{1})+c_{2}T(v_{2})+\dots+c_{k}T(v_{k})+\dots+c_{n}T(v_{n})$ 
and since $\{ v_{1},v_{2},\dots,v_{k} \}$ is a basis for nullset we get 
$w=0+c_{k+1}T(v_{k+1})+\dots+c_{n}T(v_{n})$ 
$\therefore\{ T(v_{k+1}),\dots T(v_{n}) \}=w$, the range space of $T$

Suppose that 

Theorem : Suppose that $T$ is one-to-one and $x \in N(T)$. Then $T(x) = 0 =T(0)$. Since $T$ is one-to-one, we have x — 0. Hence N(T) = {0}. 

Now assume that $N(T) = {0}$, and suppose that $T(x) = T(y)$ 
Then, $0 = T(x) - T(y) = T(x - y)$ as $T$ is linear
Therefore $x - y \in N(T) = {0}$. So $x-y = 0$, i.e  $x = y$ This means that $T$  is one-to-one. 


Let $V$ and $W$ be vectorspaces of finite dimensions, and let $T:V\to W$ be a transformation. Then the following holds 
1. T is injective 
2. T is surjective 
3. $rank(T)=dim(V)$
From rank-nullity theorem, we have nullity(T)+rank(T)=dim$(V)$ 
T is injective $\iff$ $N(T)=\{ 0 \}$ or nullity of $T$ is zero, $\implies$ nullity$(T)=0$ $\implies$ $\implies rank(T)=dim(V)=dim(V)$ 
if $V$ is finite dimensional, and $T:V\to V$ is linear, then this holds too. But not if $V$ has infinite dimensions

**Consider $P(\mathbb{R})$ be a vectorspace of all polynomial functions over $\mathbb{R}$, Let $T:P(\mathbb{R})\to P(\mathbb{R})$ by $T(f(x))=\int _{0}^xf(t) \, dt$verify if injective** 
Consider $f,g\in P(\mathbb{R})$ 
Assume $T(f(x))=T(g(x))$ then we have 
$\implies \int _{0}^x f(t)\, dt=\int _{0}^x g(t)\, dt$
$$
\begin{aligned}
\int _{0}^xf-g(t) \, dx =0\\f-g=0 \\\implies f=g
\end{aligned}
$$
T is injective.  

**Consider $P(\mathbb{R})$ be a vectorspace of all polynomial functions over $\mathbb{R}$, Let $T:P(\mathbb{R})\to P(\mathbb{R})$ by $T(f(x))=f'(x)$ verify if injective** 
Consider $f,g\in P(\mathbb{R})$ 
Assume $T(f(x))=T(g(x))$ then we have 
$\implies \int _{0}^x f(t)\, dt=\int _{0}^x g(t)\, dt$
$$
\begin{aligned}
\int _{0}^xf-g(t) \, dx =0\\f-g=0 \\\implies f=g
\end{aligned}
$$
T is injective.  
and onto ?
![[Pasted image 20250306073631.png]]


This example shows that the condition $dim(V)=dim(W)$ is necesssary 

![[Pasted image 20250306074331.png]]

Note: 
Let $V$ and $W$ be vectorspaces and $T:V\to W$ is linear, $T$ is injective $\iff$ $T$ carries linearly independent subsets of $V$ onto linearly independent subsets of $W$ 

$T$ is one one and $S$ is subset of $V$ then $S$ is linearly independent if $T(S)$ is linearly independent 

Let $V$ and $W$ be vectorspaces over $F$ and $\{ v_{1},v_{2},\dots v_{n} \}$ be a basis for $V$. For $w_{1},w_{2},\dots w_{n}$ in $W$ there exists exactly one linear transformation $T:V\to W$ and $T(v_{i})=w_{i}$ for $i=1,2,3,\dots,n$ 

![[Pasted image 20250306081331.png]]

Corollary : Let $V$ and $W$ be vectorspace and suppose that $V$ has a finite basis. If $U,T:V\to W$ are linear and $U(v_{i})=T(v_{i})$ for $i=1,2,\dots n$, then $U=T$ 

![[Pasted image 20250306082704.png]]

# The Matrix Representation of a Linear Transformation

Let $V$ be a finite dimensional vecctospace and an ordered basis for $V$ is a finite sequence of linearly independent vectors that generates $V$ 
In $\mathbb{F}^3,B=\{ e_{1},e_{2},e_{3} \}$ is a ordered basis, so is $B'=\{ e_{2},e_{1},e_{3} \}$. but $B\neq B'$ as ordered basis. 

## Ordered bases
Let $V$ and $W$ be a finite dimensional vector space over a field $F$. Let $T$ from $V\to W$ be a transformation, then $T(v_{1}),T(v_{2}),\dots T(v_{n})$ are all vectors in $W$. Since $B'=\{ w_{1},w_{2},\dots w_{m} \}$ is a basis for $W$ and $B=\{ v_{1},v_{2},\dots,v_{n} \}$ is a basis or $V$ each $T(v_{i})$ can be expressed as a linear combination of vectors from $B'$ 
$$
\begin{aligned}
T(v_{1})=a_{11}w_{1}+a_{12}w_{2}+\dots a_{1n}w_{m}\\
T(v_{2})=a_{21}w_{2}+a_{22}w_{2}+\dots a_{2n}w_{m}\\
\dots
T(v_{n})=a_{n1}w_{1}+a_{n2}w_{2}+\dots a_{nm}w_{m}
\end{aligned}
$$

Then the transformation matrix is 
$$
[T]_{B}^{B'}=\begin{bmatrix}
a_{11} & a_{12} & \dots & a_{1n} \\
a_{21} & a_{22} & \dots & a_{2n} \\
. \\
a_{m1} & a_{m2} & \dots & a_{mn}
\end{bmatrix}
$$

For each $1\leq i\leq m,1\leq j\leq n$ 
$$
T(v_{j})=\sum_{i=1}^{m}a_{ij}w_{i}
$$

We can say $A=[a_{ij}]$ is called the matrix representation of transformation (Confirm with book)

Note that $j$ column of $k$ is $[T(v_{j})]_{B'}$ ?? coordinate vector of $T(v_{j})$ wrt to basis of $W$ 

If $T,U:V\to W$ are linear transformations such that $[T]_{B}^{B'}=[U]_{B}^{B'}$, then $T=U$
## Illustration of whatever teh fuck is going on 

![[Pasted image 20250312072821.png]]

![[Pasted image 20250312074200.png]]


1. Let $V$ and $W$ be vectorspaces over field $F$ let $T,U:V\to W$ be a linear transformation, For all $a\in F$ , $aT+U$ is linear
2. Using the operations of addition and scalar multiplication in the collection of all linear transformations from $V\to W$ is a vector space over $F$ denoted by $\mathcal{L}(V,W)$ 
3. $[T+U]_{B}^{B'}=[T]_{B}^{B'}+[U]_{B}^{B'}$
4. $[aT]_{B}^{B'}=a[T]_{B}^{B'}$

Theorem, Let $V,W,Z$ be vectorspaces over same field $F$ 
Let $T:V\to W$, $U:W\to Z$ be two transformation, 
then $UT$ is a transformation given by $UT:V\to Z$ 

**Example :** In $\mathbb{R}^2$ let 

**Let $T:R_{3}\to R_{2}$ be a linear mappiing $T(x,y,z)=(2x+y-z,3x-2y+4z)$ find matrix of transformaion in following bases of $R_{3}$ and $R^2$** 
$B=\{ (1,1,1),(1,1,0),(1,0,0) \}$ 
$B'=\{ (1,3),(1,4) \}$
# Important topics

Assignment questions 
midsem question
rank nullity 
linear span and independence
matrix of transformation 
2 basis and a matrix iss given, find transformation
isomorphism of vectorspaces
basis and dimension questions 

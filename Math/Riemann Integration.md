THe idea of integration was introduced ? by Riemann and then applied by Darboux 

4 q from MI and 3 from RI
[[Bounds of a function]]

# Darboux's Lower and Upper Sum

Let $f:[a,b]\to \mathbb{R}$ be a bounded function bounded from $a\to b$  COnsider $n$ partitions to be $\{ x_0,x_1,x_2,\dots x_{i}\dots,x_n \}$ 

![[Riemann Integration 2024-12-10 12.35.35.excalidraw]]
Lower sum:  Let $m_{i}$ be the infimum for the interval $(f(x_{i-1}),f(x_{i}))$.Then the upper Darboux sum for function $f(x)$ with respect to partition $P$ is$$\sum_{i=0}^{n} m_{i}\cdot\Delta x_{i}$$ ![[Riemann Integration 2024-12-10 12.38.58.excalidraw]] Upper sum: Let $M_i$ be the supremum of $[x_{i-1},x_{i}]$. Then the upper Darboux sum for function $f(x)$ with respect to partition $P$ is $$\sum^{n}_{i=0}M_{i}\Delta x_{i}$$ note that **the width of the rectangles $\Delta x_{i}$ does not have to be uniform.** 


Let $p_{n}$ be a partion of $(a,b)$ that divides the interval into $n$ equal parts. Let $f:[a,b]\to \mathbb{R}$ be a bounded function. If $$\lim_{ n \to \infty }L(p_{n},f)=\lim_{ n \to \infty }U(p_{n},f)=l$$ for $l < \infty$, then $\int_{a}^b f \,=l$ 

The equal partition of $[a,b]$ is given by 
$$
\left\{  a,a+ \frac{b-a}{n},a+ \frac{2(b-a)}{n},a+ \frac{3(b-a)}{n},\dots ,b \right\}
$$
or 
$$\left\{  0, \frac{1}{n}, \frac{2}{n}, \dots 1  \right\}$$

 ### Show that $f(x)=x:(0,1)\int f \, dx=\frac{1}{2}$ 


First we have, 
$P_{n}=\left\{  0, \frac{1}{n}, \frac{2}{n},\dots_{1}  \right\}$ 

Giving us 
$$
\begin{aligned}
m_{i}: \inf(f(x))=\inf(x) &=x_{i-1} =\frac{i-1}{n}\\
M_{i}: \sup(f(x))=\sup(x) &=x_{i} =\frac{i}{n} \\
L(P_{n},f) =& \sum_{i=1}^n m_{i}\Delta x_{i}\\&\sum_{i=1}^n \frac{i-1}{n}\cdot \frac{1}{n}\\ &\frac{1}{n^{2}}\sum_{i=1}^n i-1\\& \frac{1}{n^{2}} \left( \frac{n(n+1)}{2}-1 \right)\\  \int_{0}^1 f \, dx =&\lim_{ n \to \infty } \frac{1}{n^{2}} \left( \frac{n\left( 1-\frac{1}{n} \right)n}{2} \right)\\=&\frac{1}{2}
\end{aligned}$$
now for upper sum, 

$$
\begin{aligned}
U(P_{n},f) =& \sum_{i=1}^n M_{i}\Delta x_{i}\\&\sum_{i=1}^n \frac{i}{n}\cdot \frac{1}{n}\\ &\frac{1}{n^{2}}\sum_{i=1}^n i\\& \frac{1}{n^{2}} \left( \frac{n(n+1)}{2} \right)\\  \int_{0}^1 f \, dx =&\lim_{ n \to \infty } \frac{1}{n^{2}} \left( \frac{n\left( 1+\frac{1}{n} \right)n}{2} \right)\\=&\frac{1}{2}
\end{aligned}
$$

### Find the limit of $\int  x^{2}\, dx$ over [0,k]


First we have, 
$P_{n}=\left\{  0, \frac{k}{n}, \frac{2k}{n},\dots{k}  \right\}$ 

Giving us 
$$
\begin{aligned}
m_{i}: \inf(f(x))=\inf(x^{2}) =x_{i-1}^{2} =&\left( \frac{(i-1)k}{n} \right)^{2}\\
M_{i}: \sup(f(x))=\sup(x^{2}) =x_{i}^{2} =&\left( \frac{ki}{n} \right)^{2}
\end{aligned}
$$
$$\begin{aligned}
L(P_{n},f) =& \sum_{i=1}^n m_{i}\Delta x_{i}\\&\sum_{i=1}^n \left( \frac{(i-1)k}{n} \right)^{2}\cdot \frac{k}{n}\\ &\frac{k^{3}}{n^{{3}}}\sum_{i=1}^n (i-1)^{2}\\& \frac{k^{3}}{n^{3}} \left( \frac{n(n+1)(2n+1)}{6}-1 \right)\\  \int_{0}^1 f \, dx =&\lim_{ n \to \infty } \frac{k^{3}}{n^{3}} \left( \frac{n\left( 1-\frac{1}{n} \right)n}{2} \right)\\=& \frac{k^{3}}{3}
\end{aligned}$$
now for upper sum, 

$$
\begin{aligned}
U(P_{n},f) =& \sum_{i=1}^n M_{i}\Delta x_{i}\\&\sum_{i=1}^n \frac{ki}{n}\cdot \frac{1}{n}\\ &\frac{1}{n^{2}}\sum_{i=1}^n i\\& \frac{1}{n^{2}} \left( \frac{n(n+1)}{2} \right)\\  \int_{0}^1 f \, dx =&\lim_{ n \to \infty } \frac{1}{n^{2}} \left( \frac{n\left( 1+\frac{1}{n} \right)n}{2} \right)\\=&\frac{1}{2}
\end{aligned}
$$

### Given an integrable $f$ prove that $kf$ is integrable

As $f$ is integrable, 
$P=\{ x_{0},x_{1},x_{2},\dots x_{n}\}$
Let $m_{i}\to \inf(f(x)):M_{i}\to \sup(f(x))$


***
If $f$ is bounded on $[a,b]$ and integrable, then 
$$
\begin{aligned}
\to \int _{a}^b f=-\int _{b}^a f\\
\to \int _{a}^af \, dx=0 
\end{aligned}
$$
# Inequality of integrals
Let $f:[a,b]\to \mathbb{R}$ be bounded and integrable, 
Let $m=\inf f(x):a\leq x\leq b$
Let $M=\sup f(x):a\leq x\leq b$

Consider $P=[x_{0},x_{1}], x_{0}=a,x_{1}=b$ 
then $\inf f(x)$

Let $f:[a,b]\to \mathbb{R}$  bounded and integrable, and $k$ be a number such that $|f(x)|\leq k,\forall x\in [a,b]$ 
Show rhat $$|\int _{a}^b f |\leq k(b-a)$$
#proof 
Given some lower bound $-k\leq f(x)\leq k$ some upper bound 
Let $m=\inf(f(x));a\leq x\leq b$
 $M=\sup(f(x));a\leq x\leq b$
Since $m$ is Greatest Lower Bound, $m\geq-k\implies m(b-a)\geq-k(b-a)$ 
and similarly as M is the Lowest Upper Bound, $M(b-a)\leq k(b-a)$
 $$
-k(b-a)\leq m(b-a)\leq \int f\leq M(b-a)\leq k(b-a) 
$$
$$-k(b-a) \leq \int f \leq k(b-a) $$
thus, $$|\int f |\leq k$$
#remark,for any number $k_{1},k_{2}$ such that $k_{1}\leq f(x)\leq k_{2} \forall x\in[a,b]$ we have $k_{1}(b-a)\leq \int f\leq k_{2}(b-a)$  

If $f,g$ are bounded and integrable on $[a,b]$ such that $f \geq g$ then show that $$\int _{a}^b \geq $$
If $f,g$ are bounded and integrable on $[a,b]$ such that $f \geq g$ then show that 
$$\int  _{a}^b f \geq \int  _{a}^b g$$
#proof  
$$
\begin{aligned}
f-g \geq 0\\f(x) -g(x)\geq 0\\\int_{a}^b f(x)-g(x) \, dx \geq 0 \\ \int_{a}^bf(x)-\int_{a}^bg(x) \geq 0\\\therefore\int_{a}^b f(x) \geq\int_{a}^b g(x)
\end{aligned}
$$

# Refinement of a partition (Property 2)
![[Pasted image 20250121123307.png]]
Of the lower sum 
We can see that more boxes have better coverage and higher sum

Let $P$ be a partition of $[a,b]$ a refinement of $P$ is partition $Q$ that contains all points of $P$ example : 
$P=\left\{  0, \frac{1}{2}, 1   \right\}$ , $Q=\left\{  0, \frac{1}{2}, \frac{2}{3}, 1  \right\}$
Let $P$ be a partition of $[a,b]$ and $Q$ be a refinement of P, Let $f: [a,b]\to \mathbb{R}$ Then, 
1. $L(P,f)\leq L(Q,f)$
2. $U(P,f)\geq U(Q,f)$

#proof 
$$
\begin{aligned}
P=\{ x_{0},x_{1},x_{2},\dots, x_{j-1} ,x_{j},\dots x_{n} \}\\
Q=\{ x_{0},x_{1},x_{2},\dots, x_{j-1},y,x_{j},\dots x_{n} \}\\ \\
m_{i}=\inf f(x), x_{i-1} \leq x \leq x_{i} \\m_{1}^y=\inf f(x), x_{j-1} \leq x \leq y\\
m_{2}^y=\inf f(x), y \leq x \leq m_{j}\\ \\
L(P,f)=m_{1}\Delta x_{1}+m_{2}\Delta x_{2}+\dots m_{j}\Delta x_{j}+\dots +m_{n}\Delta x_{n}\\
L(Q,f)=m_{1}\Delta x_{1}+m_{2}\Delta x_{2}+\dots m^y_{1}(y-x_{j-1})+m^y_{2}(x_{j}-y)+\dots +m_{n}\Delta x_{n} \\ \\
L(Q,f)-L(P,f)=m_{1}^y(y-x_{j-1})+m_{2}^y(x_{j}-y) -m_{j}(x_{j}-x_{j-1}) \\ =(m_{2}^y-m_{j})(x_{j}-y)+(m_{1}^y-m_{j})(y-x_{j-1})
\end{aligned}
$$
We prove that all 4 terms are positive
$$
\begin{aligned}
m_{2}^y \geq m_{j} \quad;\quad m_{1}^y \geq m_{j} \\ \because [x_{j-1},y],[y,x_{j}]\subseteq[x_{j-1},x_{j}]
\\\implies m_{2}^y-m_{j}\geq 0 \quad ; \quad m_{1}^y-m_{j} \geq 0\\ \therefore L(Q,f)=L(P,f)\geq 0\\\therefore L(Q,f)\geq L(P,f)
\end{aligned}
$$
and hence the difference is positive thus $L(Q,f)\geq L(P,f)$ i.e has more area and is a better approximation.


$$
\begin{aligned}
P=\{ x_{0},x_{1},x_{2},\dots, x_{j-1} ,x_{j},\dots x_{n} \}\\
Q=\{ x_{0},x_{1},x_{2},\dots, x_{j-1},y,x_{j},\dots x_{n} \}\\ \\
M_{j}=\sup f(x), x_{i-1} \leq x \leq x_{i} \\M_{1}^y=\sup f(x), x_{j-1} \leq x \leq y\\
M_{2}^y=\sup f(x), y \leq x \leq x_{j}\\ \\
U(P,f)=M_{1}\Delta x_{1}+M_{2}\Delta x_{2}+\dots M_{j}\Delta x_{j}+\dots +M_{n}\Delta x_{n}\\
U(Q,f)=M_{1}\Delta x_{1}+M_{2}\Delta x_{2}+\dots M^y_{1}(y-x_{j-1})+M^y_{2}(x_{j}-y)+\dots +M_{n}\Delta x_{n} \\ \\
U(Q,f)-U(P,f)=M_{1}^y(y-x_{j-1})+M_{2}^y(x_{j}-y) -M_{j}(x_{j}-x_{j-1}) \\ =(M_{2}^y-M_{j})(x_{j}-y)+(M_{1}^y-M_{j})(y-x_{j-1})\\ M_{2}^y \leq M_{j} \quad;\quad M_{1}^y \leq M_{j} \\ \because [x_{j-1},y],[y,x_{j}]\subseteq[x_{j-1},x_{j}]
\\\implies M_{2}^y-M_{j}\leq 0 \quad ; \quad M_{1}^y-M_{j} \leq 0\\ \therefore U(Q,f)-U(P,f)\leq 0\\\therefore U(Q,f)\leq U(P,f)
\end{aligned}
$$

It is enough to prove the result in teh situation where $Q$ has one more point than $P$ 

**Prove that $L(P_{1},f)\leq U(P_{2},f)$**

#proof  Let $P_{1}$ and $P_{2}$ be any 2 partitions of closed interval $a,b$ and $f:[a,b]\to \mathbb{R}$ be bounded. Then, consider $Q=P_{1} \cup P_{2}$ we can see that $Q$ is a refinement of $P_{1}$ and $P_{2}$ thus, by previous property

wkt, $L(P_{1},f)\leq L(Q,f)$ and $U(Q,f)\leq U(P_{2},f)$ .. and $L(Q,f)\leq U(Q,f)$ so, 
 $$
L(P_{1},f)\leq L(Q,f) \leq U(Q,f)\leq U(P_{2},f)
$$
$\therefore L(P_{1},f)\leq U(P_{2},f)$ 

# Property 3 - Let $f:[a,b]\to \mathbb{R}$ be bounded, then we can say $\int _{\bar{a}}^b f \leq \int _{a}^\bar{b}$ 

Let $P$ and $Q$ be two partitions of $[a,b]$ then $L(P,f)\leq U(Q,f)$ by property 2. 
Fix $Q$ and let $P$ vary over all partitions of $a,b$  then $U(Q,f)$ is an upper bound of $L(P,f)$ for all $P$. $U(Q,f)$ is greater than the least upperbound of all $L(P,f)$. and the least upper bound =$\int _{\bar{a}}^b f$. 
Now if we vary $Q$ over all partitions, of $[a,b]$ then we get $\int _{\bar{a}}^b f\leq U(Q,f)$  and is a lower bound for all $Q$ it is lower than greatest ower bound of all $U(Q,f)$ but this $GLB$ is just $\int _{a}^{\bar{b}}f$ thus we have 

# Norm of the partition
Let $P=\{ x_{0},x_{1},x_{2},\dots_{n} \}$ where they are patition of $[a,b]$ the norm of the partition is given by $||P||$ or $\mu(P)$. $$\mu(P)=max\{ \Delta x_{i} \}$$ 

# Darboux theorem

If $f:[a,b]\to \mathbb{R}$ is a bounded function, on closed interval $[a,b]$ then for every $\epsilon \geq 0$ there exists $\delta \geq 0$ succh that 
1. $U(P,f)<\int _{a}^{\bar{b}}f+\epsilon$
2. $L(P,f)>\int _{\bar{a}}^{b}f-\epsilon$
for evry partition P with $\mu(P)<\delta$ 
 -- MIDSEM
## Condition for integrability,
Let $f:[a,b]\to \mathbb{R}$ be bounded function, then $f$ is integrale iff $\forall\epsilon >0:\forall$ partition $P[a,b]$ with $\mu(P)<\delta$ we have $U(P,f)-L(P,f)<\epsilon$ 
this theorem says that when partiotion size is small, the difference between upper and lower sums for that partition should be small. 
 
 #remark  $$\lim_{ \mu(P) \to 0 }U(P,f)=\lim_{ \mu(P) \to 0 }L(P,f)=\int _{a}^bf  $$ if both limits exist and are equal. 

Another criteria could be : 
Let $f:[a,b]\to \mathbb{R}$ be bounded function, then $f$ is integrable iff $\forall\epsilon>0\exists$ a partitiion $P$ of $[a,b]$ for which $U(P,f)-L(P,f)<\epsilon$ 

# Monotocity 

A function is said to be monotonic if it is either monotonically increasing or decreasing 
## Increasing
let $a\subseteq \mathbb{R}$ then the function is monotonously increasing if $f(x_{2})\geq f(x_{1})$ for all $x_{2}\geq x_{1}$. or $f$ increases with $x$ 
## Decreasing
let $a\subseteq \mathbb{R}$ then the function is monotonously decreasing if $f(x_{2})\leq f(x_{1})$ for all $x_{2}\geq x_{1}$. or $f$ increases with $x$ 

#proof **Monotonic functions are integrable** 

A non const monotonic function $f:[a,b]\to \mathbb{R}$ is integrable.. We may first assume $f$ is monotonically increasing and $p$ be any partition $x_{0},x_{1},\dots x_{n}$ 
Let $m_{i}=\inf f(x)=f(x_{i-1}):x_{i-1}\leq x\leq x_{i}$
Let $M_{i}=\sup f(x)=f(x_{i}):x_{i-1}\leq x\leq x_{i}$

$$
\begin{aligned}
U(p,f)=&\sum M_{i}\Delta x_{i}\\=&\sum f(x_{i})\Delta x_{i}\\P(p,f)=&\sum m_{i}\Delta x_{i}\\=&\sum f(x_{i-1})\Delta x_{i}\\ \\ U(p,f)-L(p,f)=&\sum(f(x_{i})-f(x_{i-1}))\Delta x_{i} \\ <&\sum(f(x_{i})-f(x_{i-1}))\delta  \\ <&[(f(x)-f(x_{0}))+(f(x_{2})-f(x_{1}))+(f(x_{3})-f(x_{2}))\dots f(x_{n})-f(x_{n-1})] \delta\\ <&f(x_{n})-f(x_{0})\delta \\ \\ &\text{Let $\delta=\frac{\epsilon}{f(x_{n}-f(x_{0}))}$ }\\ \implies U(p,f)-L(p,f)< & f(x_{n})-f(x_{0}) \frac{\epsilon}{f(x_{n}-f(x_{0}))} \\<\epsilon
\end{aligned}
$$

 for any value of $\delta$ lower than this, the function is integrable.. ? Suppose $\epsilon>0$ is given, then we have to find $\delta > 0$ with $\mu(p)<\delta$ in this case we choose a $\delta$ as above to ensure that $P$ has enough points so that $\Delta x_{i}\leq \mu(P)\leq\delta$ hence $f$ is integrable. 

Similarly, for a decreasing function : 
let $f$ be a monotonically decreasing function, then $-f$ is an increasing function i.e integrable as shown, thus $-(-f)$ must also be integrable as we saw integrability of $f\implies$ integrability of $kf$ 

# Continuous function 
let $a\subseteq \mathbb{R}$ and a function $f:a\to \mathbb{R}$ is said to be continuous at point $x_{0}$ if given an $\epsilon > 0$ there exists $\delta>0$ such that for $x\in a$ with $|x-x_{0}|<\delta$ 

If $f,g$ are  


# Fundamental thorem of calculus 

Let $F$ be teh primitive of $f$ then $\int _{a}^b f=F(b)-F(a)$ and let $P=\{ x_{0},x_{1},x_{2}\dots \}$  be the partition of $f$ and it is continuous on all intervals $[x_{i-1},x_{i}]$ 
Lagrange's Mean Value Theorem gives us tp-0o90i8uyhjy7yiokp900piiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiiii98
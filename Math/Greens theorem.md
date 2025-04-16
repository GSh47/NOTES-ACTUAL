If $R$ is closed region bounded by simple clsoed curve C and $m(x,y)$ and $n_{x,y}$ are two functions having continuous partial derivatives in $R$ then
$$
\oint_{C}Mdx+Ndy=\iint_{R} \left( \frac{ \partial N }{ \partial x } -\frac{ \partial M }{ \partial y }  \right)dxdy  
$$
integrated in anti clockwise 
the lines parlell to thn coord axis meets the boundary of the curve C, at no more than $2$ points. The figure 
![[Greens theorem 2025-03-10 08.12.51.excalidraw]]
Shows that $C$ is made up of two path $C_{1}:y=f_{1}(x),C_{2}:y=f_{2}(x)$ now for any $x$ between $a,b$ we integrate $\frac{ \partial M }{ \partial y }$ with $y$ from $y=f_{1}(x)$ to $f_{2}(x)$ i.e $\int _{f_{1}(x)}^{f_{2}(x)}\frac{ \partial M }{ \partial y } \, dy$ and let hte integral be $\mathbb{M}(x,y)|_{f_{1}(x)}^{f_{2}(x)}$ 
and we integrate it with $x$ from $a,b$ i.e $\int _{a}^b \, \mathbb{M}(x,y)|_{f_{1}(x)}^{f_{2}(x)}dx$ or 
$$
\int _{a}^b \, \mathbb{M}(x,f_{2}(x))-\mathbb{M}(x,f_{1}(x))dx = 
\int _{a}^b \, \mathbb{M}(x,f_{2}(x))dx+\int _{b}^a \mathbb{M}(x,f_{1}(x))dx
$$
Similarly along for $N$ 
$C_{1}':x=g_{1}(y)$ for $d\leq y\leq c$ and $C_{2}'=g_{2}(y)$ for $c\leq y\leq d$ 
we integrate $\frac{ \partial N }{ \partial x }$ along the curves
$$
\begin{aligned}
\int _{c}^d \int _{g_{1}(y)}^{g_{2}(y)} \frac{ \partial N }{ \partial x }  \, dx \, dy\\\
\int _{c}^d \mathbb{N}(g_2(y),y)-\mathbb{N}(g_{1}(y),y) \, dy\\
=\int _{c}^d \mathbb{N}(g_2(y),y)dy+\int _{d}^c\mathbb{N}(g_{1}(y),y) \, dy
\end{aligned}
$$

which is just $\oint_{c}N(x,y)dy$ 

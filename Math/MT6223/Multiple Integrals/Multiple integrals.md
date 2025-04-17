# Double integrals

In case of a single variation function, integration is taken only once but if there are two or more independent variables, then we consider the integration twice or more times respectively - such are double and integral multiples. 
A double integral is represented as 
$$
\int_{x_{1}}^{x_{2}} \int_{y_{1}}^{y_{2}} f(x,y)  \, dy  \, dx 
$$

# Evaluating a double integral 
Consider double integral of the form $\int_{x_{1}}^{x_{2}} \int_{y_{1}}^{y_{2}} f(x,y)  \, dy  \, dx$. We can have 3 cases. 
## Case 1: y is dependent on x
#note: outer integral is a constant. 
![[Multiple integrals 2024-12-05 11.56.01.excalidraw]]
$$
\int ^{x_{2}}_{x_{1}}\int ^{f_{2}(x)}_{f_{2}(x)} f(x,y)\, dy  \, dx 
$$
## Case 2: x is dependent on y
$$\int ^{y_{2}}_{y_{1}}\int ^{f_{2}(y)}_{f_{2}(y)} f(x,y)\, dx  \, dy $$



[[problems on multiple integrals]] 

Suppose a continuous function $z=f(x,y):a\leq x\leq b;c\leq y\leq d$ representing a surface in the 3d Space and a region in the xy plane. 
Thne double integral measures **volume** between the surface given by function and the **rectanglular region R** (Fubini's Theorem) 

If $f(x,y)$ is a continuous function of $x\&y$ and $f(x,y)>0$ over teh rectangle, then we have $$V=\int _{a}^b \int _{c}^d f(x,y)\, dy \, dx=\int _{c}^d \int _{a}^b f(x,y)\, dx \, dy $$ 
Example :  
$$
\begin{aligned}
\int \int \cos(x+2y) \, dA \\R=\left\{  (x,y)|0\leq x\leq \pi, 0\leq y\leq \frac{\pi}{2}  \right\}
\end{aligned}
$$


# Using horizontal cross section. 
Imagine horizontal strip cutting through $R$ in direction of $x$ mark the $x$ values where the horizontal region enters and leaves the regions. these are the x limits of integration which are functions of $y$ 

choose $y$ limits that include horizontal lines through R
Since integration is wrt $x$ then wrt $y$ then we have 
$$
\begin{aligned}
\int \int_{R} f(x,y)    \, dA \\ \int _{y=c}^d \int _{x=h_{1}(y)}^{x=h_{2}(y)} f(x,y) \, dx \, dy 
\end{aligned} 
$$

# Evaluation of double integral by changing of orders 

You rewrite the vriables in the form of other 
$$
\int ^{x_{2}}_{x_{1}}\int ^{f_{2}(x)}_{f_{2}(x)} f(x,y)\, dy  \, dx\longrightarrow \int ^{y_{2}}_{y_{1}}\int ^{f_{2}(y)}_{f_{2}(y)} f(x,y)\, dx  \, dy 
$$
# Area bounded by double integral
Area bounded by plane region $R$ is given by $\int \int  dA$

# Average value of function of two variables

To compute the average value of the function $f(x):[a,b]$ we compute the integral of $f$ over the given interval and divide it by range or length of integral.
The area of the function in a 2D space divided by length : $$\langle f(x) \rangle=\left( \frac{1}{b-a} \right)\int _{a}^a f(x)\, dx  $$
if $f(x,y)$ is a positive function over region $R$ then the double integral measures the volume under the surface. If we divide this volume by the area of the region, we get the average value of $f(x,y)$ over $R$ $$\langle f(x,y) \rangle=\frac{1}{A} \iint _{R} f(x,y) \, dA  $$
If we divide the volume of the enclosed space by the area of the base, we get the height of the box. 

# Double integration by change of variables
Sometimes it's easier to integrate in a different coordinate system, like the polar coordinate system. 
We can switch with $x=r\cos\theta$ and $y=r\sin\theta$ 
and we must compute the jacobian when switching to a different coordinate system like cartesian, polar, sphereical, cylindrical etc 
$$
J=\begin{vmatrix}
\frac{ \partial x }{ \partial r }  & \frac{ \partial x }{ \partial \theta } \\
\frac{ \partial y }{ \partial r } &\frac{ \partial y }{ \partial \theta }  
\end{vmatrix}
$$
giving us $dxdy=Jdrd{\theta}$ which is $rdr{\theta}$

# Triple integral 
A triple integral can be evaluated by changing the variable $x,y,z$ to some new variables related to $x,y,z$. as long as the Jacobian is not zero
$$
\iiint f(x,y,z) dx dydz \to \iiint g(u,v,w) \,\,|J| \,\,dudvdw
$$
there are two particular trasofrmations : 
1. Cylindrival polar coords $(x,y,z)\to(r,\theta,z)$ 
	by the relation $(x=r\cos\theta,y=r\sin\theta,z=z)$ 
2. Sphereical polar coords $(x,y,z)\to(r,\phi,\theta)$ by the relation $(x=r\sin \phi \cos \theta,y=r\cos\theta \sin \phi,z=r\cos \phi)$

$$
\begin{aligned}
J&=\begin{vmatrix}
\frac{\partial x}{\partial r} &
\frac{\partial y}{\partial r} &
\frac{\partial z}{\partial r} \\
\frac{\partial x}{\partial \theta} &
\frac{\partial y}{\partial \theta} &
\frac{\partial z}{\partial \theta} \\
\frac{\partial x}{\partial \phi} &
\frac{\partial y}{\partial \phi} &
\frac{\partial z}{\partial \phi}
\end{vmatrix} \\&=
\begin{vmatrix}
\sin{\theta}\cos{\phi} &
\sin{\theta}\sin{\phi} & \cos{\theta} \\
r\cos{\theta}\cos{\phi} &
r\cos{\theta}\sin{\phi} & -r\sin{\theta} \\
-r\sin{\phi}\sin{\theta} &
r\cos{\phi}\sin{\theta} & 0
\end{vmatrix}\\&=r^{2}\sin\phi
\end{aligned}
$$
Q **Evaluate $\iiint\sqrt{ x^{2}+y^{2} }dxdydz$ using cylindrical coordinates where $R$ is a region lying between cylinder $x^{2}+y^{2}=16$ and planes $z:-5,4$**

it can be rewritten as an integral in cylindrical coords 
$$
\begin{aligned}
\to \int _{-5}^4 \int _{0}^4 \int _{0}^{2\pi} \,r d\theta \, dr \, dz \\=\int _{-5}^4 \int _{0}^4 2\pi \, rdr \, dz \\=\int _{-5}^4  \frac{2\pi \,r^{2}}{2} |_{0}^4 \, dz=\int _{-5}^4  \pi \cdot{1}6 \, dz\\=\int _{-5}^4  \pi \cdot{1}6 \, dz\\ =  \pi \cdot{1}6z|_{-5}^4\\=\pi \cdot 16 \cdot{9}\\ 
\end{aligned}
$$
**Evaluate $\int _{-1}^1 \int _{-\sqrt{ 1-x^{2} }}^{\sqrt{ 1-x^{2} }}\int _{0}^2 \sqrt{ x^{2}+y^{2} }\, dz \, dy\, dx$**

# Important limits when integratng 
1. Spherically 
$$
\begin{matrix}
r & 0\to a \\
\theta & 0\to{2}\pi \\
\phi  & 0\to 0\to \pi
\end{matrix}
$$

2. SemiSphere
$$
\begin{matrix}
r & 0\to a \\
\theta & 0\to{2}\pi \\
\phi  & 0\to 0\to \frac{\pi}{2}
\end{matrix}
$$


**Find volume of the Sphere $x^{2}+y^{2}+z^{2}=a^{2}$** 
by changing to sphereical polar coords 
- First find Jacobian = $r^{2}\sin \phi$ 
- rhus vol = 
$$
\int^{a} _{0}\int^{\pi} _{0}\int^{2\pi} _{0} r^{2}\sin \phi d\theta d\phi\ dr 
$$
is obviously $\frac{4}{3}\pi a^{3}$ where $r^{2}\to \frac{a^{3}}{3}$ ; $\sin \phi\to \cos \phi|_{0}^{\pi}\to1-(-1)=2$ and we just get $2\pi$ from the theta integral 

integrate $\iiint(x+y+z)dxdydz$ in the first octant bounded by the sphere 

**Find area of trapezoid in first octant :** $6x+4y+3z=12$ 

The limits are found by subs 0 to other two vars when checking value
$$
\begin{aligned}
6x=12\to x=2\\4y=12\to y=3\\3z=12\to z=4
\end{aligned}
$$
as upper lims and subs required var to zero to get lower lims
$$
\begin{aligned}
4y+3z=12\to x=\frac{1}{3}(4y+3z-12)\\3z=12\to y=\frac{1}{4}(3z-12)\\3z=12\to z=4
\end{aligned}
$$

thus $\int_{0}^4 \int _{0}^{1/4(3z-12)}\int _{0}^{1/3(4y+3z-12)} \, dx \, dy \, dz$ 
we get it to be 4 

Find vol bounded by ylinder $x^{2}+y^{2}=4$ and the plane $y+z=3$ and $z=0$ 

**Evaluate by double integrals, the volume generated by the revolution of the carioid**
$r=1-\cos\theta$ about it's axis 

and the vlume is $\iint 2\pi r^{2}\sin\theta drd{\theta}$ 
the limits are 
$$
\begin{aligned}
\int _{0}^\pi \int _{0}^{a(1-\cos\theta)}2\pi r^{2}\sin\theta \, dr \, d\theta\\ 
\end{aligned}
$$

The double integral can be made use to evaluate the surface area of the surface it can be shown that the area of the surface is given by 
$$
S=\iint\left[ 1+\left( \frac{ \partial z }{ \partial x }  \right)^{2}+\left( \frac{ \partial z }{ \partial y }  \right)^{2} \right]^{1/2} dx dy
$$
Where a is a projection of surface S onthe $xy$ plane, similarly, if $b$ is a projction of $S$ on the $yz$ plane, 
$$
S=\iint\left[ 1+\left( \frac{ \partial x }{ \partial y }  \right)^{2}+\left( \frac{ \partial x }{ \partial z }  \right)^{2} \right]^{1/2} dy dz
$$

and of c is a rojecion of $xz$ plane 
$$
S=\iint\left[ 1+\left( \frac{ \partial y }{ \partial x}  \right)^{2}+\left( \frac{ \partial y }{ \partial z }  \right)^{2} \right]^{1/2} dx dz
$$


**Find the surface area of the sphere $x^{2}+y^{2}+z^{2}=4$ the total surface area of the sphere is** $8$ **times the surface area of the positive octet of the sphere. the projection of this on the $xy$ plane is the region $a$ in the positive quadrant of the circle $x^{2}+y^{2}=4$** 

Given a sphere of the $z^{2}=4-x^{2}-y^{2}$ or just $z=\sqrt{ 4-x^{2}-y^{2} }$ 

Total surface area is given to be 
$$S=8\iint\left[ 1+\left( \frac{ \partial z }{ \partial x }  \right)^{2}+\left( \frac{ \partial z }{ \partial y }  \right)^{2} \right]^{1/2} dx dy
$$
we differentiate the $z^{2}$ thing to get an expression $\frac{ \partial z }{ \partial x }=-\frac{x}{z}$  and similarly for $y$ we get $\frac{ \partial z }{ \partial y }=-\frac{y}{x}$


We use idea of coord transforms to evaluate substituitions to evaluate integrals by substituition, We replace complicated integrals with those that are easier to evaluate by simplifying the integrand, the limits of integration or both. 

The equation $x=g(u,v)$ and $y=h(u,v)$ allows us to change an integral over region $R$ inthe $x,y$ plane into an integral over region $S$ in the $u,v$ plane  
$$
\iint f(x,y)dxdy=\iint f(g(u,v),h(u,v))|J|dudv
$$
**Find the jacobian for polar transformation $x=rcos\theta;y=r\sin\theta$ and hte cartesian integral $\iint f(x,y)dxdy$ as a polar integral.** 


# Greens Theorem
[[Greens theorem]] Double integral over a plain region can be transformed into a line integral over a boundary of the region and conversely
# Stokes Theorem 
[[Stokes theorem]] is the relation between a line integral and a surfce integral

# Gauss Divergence 

If $V$ is a volume bounded by closed surafce $S$ and $\vec{F}$ is a vector point function with continuous derivatives in $v$ then $$\iint\vec{F}\cdot \hat{n}ds=\iiint \nabla \cdot \vec{F}dV$$ where $\hat{n}$ is the outward pointing vector 

#proof Let $\vec{F}=F_{1}\hat{i}+F_{2}\hat{j}+F_{3}\hat{k}$ 
and their derivatives are continuous at all points in $V$ Now, 
$\nabla \cdot \vec{F}=\left( \frac{ \partial F_{1} }{ \partial x } \right)+\frac{ \partial F_{2} }{ \partial y }+\left( \frac{ \partial F_{3} }{ \partial z } \right)$ 

and on other side, 
$\iint(F_{1}\hat{i}\cdot \hat{n}+F_{2}\hat{j}\cdot \hat{n}++F_{3}\hat{k}\cdot \hat{n})ds$ or
$\iint(F_{1}\hat{i}\cdot \hat{n}ds+\iint(F_{2}\hat{j}\cdot \hat{n})ds+\iint F_{3}\hat{k}\cdot \hat{n}ds$ 
Let $S$ be a closed surface such that any line parallel to any coord axis cuts the surface $S$ in atmost $2$ points. Let $R$ be the orthogonal projection of the surface $S$ on the $xy$ plane. 



![[Multiple integrals 2025-03-20 11.21.02.excalidraw]]

A line through the point $x,y,0$ of $R$ meets teh boundary of $S$ at two points Let the $Z$ coordinates of these points be $z_{1}=f_{1}(x,y),z_{2}=f_{2}(x,y)$  Let us denote the position of the surface $S$ corresponding to $z=f_{1}(x,y),z=f_{2}(x,y)$ as $S_{1},S_{2}$ respectively

Let $\hat{n_{1}},\hat{n}_{2}$ be the unit normal drawn outward to $S_{1},S_{2}$ such that $dxdy=-\hat{k}\cdot \hat{n_{1}}ds_{1}$ and $dxdy=\hat{k}\cdot \hat{n_{2}}ds_{2}$ 

Consider the integral $\iiint \frac{ \partial F_{3} }{ \partial z }dxdydz$ 

we have $$
\begin{aligned}
\iint \frac{ \partial F_{3} }{ \partial z }|_{f_{1}(x,y)}^{f_{2}(x,y)}dxdy
\end{aligned}
$$
Adding $5,6,7$ ?

# 
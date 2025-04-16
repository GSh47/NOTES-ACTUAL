### Differential equation
An equation involving derivatives of one or more dependent variables with respect to one or more independent variables is called a differential equation 
### Ordinary Differential Equation 
Differential equation involving derivatives wrt single variable is called ODE 
Examples : 
$\frac{dy}{dx}=x+\sin(x)$
$\frac{d^4x}{dt^4}+\frac{d^2x}{dt^2}+\left( \frac{dx}{dt} \right)^5=e^t$
### Partial Differential Equation 
A differential equation involving partial derivatives with respect to more than one independent variable is called partial differential equation
examples 
$\frac{ \partial^{2} v }{ \partial t ^{2}}=k^{2}\left( \frac{ \partial v ^{3}}{ \partial t^{3} } \right)$
$\frac{ \partial T(x,y) }{ \partial x }+\frac{ \partial T(x,y) }{ \partial y }$
### Order of differential equation 
Order of highest order derivative involved in a differential equation is called the order of differential equation
### Degree of differential equation 
the degree of differential equation is the highest degree or power of the highest derivative, which occurs in it. after the differential equation has been made free from radicals ($n$th root) and fraction as far as the derivatives are concerned. 
### Solution of Differential equation 
Any relation between dependent and independent variable which when substituted in the differential equation reduces it to an identity is called a solution or integral of differential equation.

### General solution of differential equation
Let $F(x_{1},y_{1},y_{2},\dots y_{n})=0$ be a nth order differential equation. 
A solution containing $n$ independent arbitrary independent constants is called a general solution. 
Family of curves basically 
### Particular Solution
A solution obtained from general solution by substituting particular values to one or more of the independent variables hence finding the value of arbitrary constants is called Particular solution. 
### Singular solution 
A solution which cannot be obtained from the general solution of the equation by any choice of $n$ arbitrary indepndent constants is called singular solution

example : 
Consider $\left( \frac{dy}{dx} \right)^{2}-4y=0$ the general solution is $y=(4x+c)^{2}$ 
now 


# Solving PDE's
## General method
**Consider $(y^{2}+yz)dx+(xz+z^{2})dy+(y^{2}-xy)dz=0$**

Now, Let $z$ be constant - $dz=0$ 
$$
\begin{aligned}
(y^{2}+yz)dx+(xz+z^{2})dy=0\\
y(y+z)dx+z(x+z)dy=0\\
-\frac{dx}{z(x+z)}=\frac{dy}{y(y+z)}
\end{aligned}
$$
Resolve RHS into Partial fraction 
$$
\begin{aligned}
-\int\frac{dx}{z(x+z)}=\int  \frac{dy}{(y+z)}-\int  \frac{dy}{y}\\
\log(x+z)-\log(y+z)+\log y=\log c\\ \log\left( \frac{y(x+z)}{y+z} \right)=c\\
\implies \frac{y(x+z)}{y+z}=F(z)
\end{aligned}
$$
now, take a total derivative of this, compare with original question, to get an expression in terms of $F(z)$, subs that here to get final answer
Now 

## Solution by inspection
Used if we can rewrite terms in the equation as a derivative of something else

Sometimes by rearranging the terms of the given equation and/or by dividing a suitable function of $x,y,z$, the equation thus obtained will contain several parts that are exact differentials. 
example 
$$
\begin{aligned}
d(xy)=&xdy+ydx\\d(x^{2}+y^{2})=&2xdx+2ydy\\d(xyz)=&xydz+azdy+yzdx\\d(x^{2}+y^{2}+z^{2})=&2(xdx+ydy+zdz)\\d\left( \frac{y}{x} \right)=&\frac{xdy-ydx}{x^{2}}\\d\left( \ln\left( \frac{y}{x} \right) \right)=&\frac{x}{y}d\left( \frac{y}{x} \right)=\frac{xdy-ydx}{xy} \\ d\left( \arctan\left( \frac{y}{x} \right) \right)=&\frac{xdy-ydx}{x^{2}+y^{2}}\\d(x^{2}y)=&y^{2}dx+2xydy\\d(x^{2}y)=&x^{3}dy+3yx^{2}dy \\d\left( \frac{y^{2}}{x} \right)=&\frac{2xydy-y^{2}dx}{x^{2}}
\end{aligned}
$$
**Solve $(yz+xyz)dx+(zd+xyz)dy+(xy+xyz)dz=0$** 

Condition of integrability : check for derivtives of $P,Q,R$ 
$$
\begin{aligned}
P=&yz+xyz&\frac{ \partial P }{ \partial y } =z+xz&&\frac{ \partial P }{ \partial z }=y+xy
\\Q=&zx+xyz & \frac{ \partial Q }{ \partial x } =z+yz && \frac{ \partial Q }{ \partial z } =x+xy
\\R=&xy+xyz & \frac{ \partial R }{ \partial x } =y+yz && \frac{ \partial R }{ \partial y } =x+xz
\end{aligned}
$$
we have 
$$
\begin{aligned}
&P\left( \frac{ \partial Q }{ \partial z } -\frac{ \partial R }{ \partial y }  \right)+Q \left(\frac{ \partial R }{ \partial x } -\frac{ \partial P }{ \partial z }\right) +R\left( \frac{ \partial P }{ \partial y } -\frac{ \partial Q }{ \partial x }  \right)\\
=&xyz[(1+x)(y-z)+(1+y)(z-x)+(1+z)(x-y)]\\
=&0
\end{aligned}
$$
$\therefore$ it is integrable, 
Consider $(yz+xyz)dx+(zd+xyz)dy+(xy+xyz)dz=0$ nd now divide by $xyz$ 
$$
\begin{aligned}
\left( \frac{1}{x} +1\right)dx+\left( \frac{1}{y} +1\right)dy+\left( \frac{1}{z} +1\right)dz\\\text{integrate to get: } \\\log(x)+\log(y)+\log(z)+x+y+z=c \\log(xyz)+x+y+z=c
\end{aligned}
$$

# Simultaneous Differential equation

Consider two PDEs in 3 variables 
$$
\begin{aligned}
P_{1}dx +Q_{1}dy+R_{1}dz=0\\P_{2}dx +Q_{2}dy+R_{2}dz=0
\end{aligned}
$$

When coeffs are functions of $x,y,z$ then solving these equations simultaneously we have $$\frac{dx}{Q_{1}R_{2}-Q_{2}R_{1}}= \frac{dy}{R_{1}P_{2}-R_{1}P_{1}}=\frac{dz}{P_{1}Q_{2}-P_{2}Q_{1}}$$ 
Which is just $$\frac{dx}{P}=\frac{dy}{Q}=\frac{dz}{R}$$ called a Simutaneous differential equation

Given equations are said to be compeletely solved when we get a solution of the form 
$$
\begin{aligned}
u_{1}(x,y,z)=c_{1}\\u_{2}(x,y,z)=c_{2}
\end{aligned}
$$
There are three methods of solving : 
## First Method ?
Consider two ratios and solve it to get the solution 
$$
\frac{dx}{P}=\frac{dy}{Q}\to u_{1}(x,y,z) \quad u_{2}(x,y,z)\leftarrow\frac{dy}{Q}=\frac{dz}{R}
$$

**Solve $\frac{dx}{x^{2}+2y^{2}}=\frac{dy}{-xy}=\frac{dz}{xz}$** 

Consider $\frac{dy}{-xy}=\frac{dz}{xz}$
$$
\begin{aligned}
\int \frac{dy}{-xy}=\int   \frac{dz}{xz} \\ \log(c_{1})=\log z+\log y\\ \log (c_{1})=\log (zy)\\c_{1}=zy
\end{aligned}
$$
and now the other two
Consider $\frac{dy}{-xy}=\frac{dx}{x^{2}+2y^{2}}$, 
=$\frac{dy}{dx}=-\frac{xy}{x^{2}+2y^{2}}$ 
this is a [[homogenous equation]]  - solve (subs $y=vx$)
to get $vx^{2}\sqrt{ 1+v^{2} }=c_{2}'$ now plug $\frac{y}{x}=v$ to get $y\sqrt{ x^{2}+y^{2} }=c_{2}'$ and ofc, square it to be nice

## Method 2
Suppose only one relation of the form $u_{1}(x,y,z)=c_{1}$ can be found by method 1, then we will use this relation in expressing one variable in terms of the other. The solution of this equation will give us the second relation for the general solution of the simultaneous diff eq. which will involve arbitrary constant $c_{1}$ which must be removed with the help of the first relation. 

Solve $\frac{dx}{xz}=\frac{dy}{yz}=\frac{dz}{xy}$ 
Consider any two ratios, 
$$
\begin{aligned}
\frac{dx}{xz}= \frac{dy}{yz}\\\implies \int  \, \frac{dx}{x}- \int  \, \frac{dy}{y}=0\\ 
\log(x) -\log(y)=\log c_{1}\\\implies \frac{x}{y}=c_{1}\end{aligned}
$$

is our first solution
$$
\begin{aligned}
Consider \frac{dx}{xz}=\frac{dz}{xy}\\ \frac{dx}{z}=\frac{dz}{y}=\frac{c_{1}dz}{x}\\ \implies xdx=c_{1}zdz\\ \frac{x^{2}}{2}- \frac{c_{1}z^{2}}{2}=c_{2} \\\implies \frac{x^{2}}{2}-\left( \frac{x}{y} \right) \frac{z^{2}}{2}=c_{2}\\ \implies x^{2}y-xz^{2}=yc_{2}
\end{aligned}
$$
is our second solution

## Method of multipliers

Consider $\frac{dx}{P}= \frac{dy}{Q} = \frac{dz}{R}$ which is equal to some $\mu$. Let $P_{1},Q_{1},R_{1}$ be functions of $x,y,z$ then 
$$
\frac{P_{1}dx+Qdy+Rdz}{P_{1}P+Q_{1}Q+R_{1}R}=\mu
$$

\If $P_{1}P+Q_{1}Q+R_{1}R=0$ then integrating $P_{1}dx+Q_{1}dy+R_{1}dz=0$ gives us the solution $u_{1}(x,y,z)=c_{1}$. $P_{1},Q_{1},R_{1}$ are called multipliers

We find another set of multipler $P_{2}P+Q_{2}Q+R_{2}R=0$ and thus $P_{2}dx+Q_{2}dy+R_{2}dz=0$ gives us another solution $u_{2}(x,y,z)$ 

Example. Solve $\frac{dx}{x(y-z)}= \frac{dy}{y(z-x)} = \frac{dz}{z(x-y)}$ 
Choose $(1,1,1)$ as our first set of multipliers 
$$
\begin{aligned}
\frac{dx+dy+dz}{xy-xz+yz-yx+zx-zy}=\mu\\\implies \int  \, dx+\int  \, dy +\int  \, dz=0\\x+y+z=c_{1}  
\end{aligned}
$$
and now choosing $\left( \frac{1}{x}, \frac{1}{y}, \frac{1}{z} \right)$ as second set of multipliers
$$
\begin{aligned}
\int \, \frac{dx}{x}+ \int  \, \frac{dy}{y} + \int  \, \frac{dz}{z}=0\\ \log(x)+\log(y)+\log(z)=\log c_{2}\\ \log(xyz)=\log(c_{2}) \\xyz=c_{2} 
\end{aligned}
$$


**Solve** $\frac{dx}{x^{2}-y^{2}-z^{2}}= \frac{dy}{2xy}=\frac{dx}{2xz}$ 

THe second and third are easuly solved to get $\frac{y}{z}=c_{1}$ and then we take $(x,y,z)$ as multipliers. 

# Partial Differential Equations 
Z is a dependent variable (or multivariate function ?)
An equation containing one or more partial derivatives of an unknown function of two or more independent variables is known as **partial differential equation.** 

- The **Order** of a PDE is the highest order partial derivative occurring in the PDE
- The **degree** of a PDE is the degree of the highest order derivative, which occurs in it after the equation has been made free from radicals and fractions as far as derivatives as concerned. 
- A partial differential equation is said to be **linear PDE** if the dependent variable and it's partial derivatives occur only in the first degree and are not multiplied 
- A PDE that is non linear is called a **non linear PDE**

example : 
$\frac{ \partial z }{ \partial x }+\frac{ \partial z }{ \partial y }=z+xy$ this is linear

$\left( \frac{ \partial z }{ \partial x } \right)^{2}+\frac{ \partial^{3} z }{ \partial y^{3} }$ is non linear higher order and higher degree

$z \frac{ \partial z }{ \partial x }+\frac{ \partial z }{ \partial y }=x$ is non linear as $z \cdot \frac{ \partial z }{ \partial x }$ is dep.var multiplied by derivattive.. hencce making it non linear

### Notations
$$
\begin{matrix}
p & \frac{ \partial z }{ \partial x }  \\
q & \frac{ \partial z }{ \partial y }  \\
r & \frac{ \partial^{2} z }{ \partial^{2} x } \\
t & \frac{ \partial^{2} z }{ \partial^{2} y }  \\
s & \frac{ \partial^{2} z }{ \partial x \partial y } 
\end{matrix}
$$

# Formation of PDEs
### By eliminating arbitrary const
Consider an equation of the form $$F(x,y,z,a,b)=0$$ where $a,b$ are arbitrary constants, let $z=F(x,y)$ Diff the equation partially wrt to $x$
$$
\frac{ \partial F }{ \partial x } +\frac{ \partial F }{ \partial z } \frac{ \partial z }{ \partial x } =0
$$
note that $\frac{ \partial F }{ \partial y }=0$. Differentiate 1 partially wrt y
$$
\frac{ \partial F }{ \partial y } +\frac{ \partial F }{ \partial z } \frac{ \partial z }{ \partial y } =0
$$
and we eliminate $a ,b$ with the two diff eqs 

**FOrm the PDE by eliminating arbitrary constants,** : $z=(x^{2}+a)(y^{2}+b)$
$$
\begin{aligned}
z=(x^{2}+a)(y^{2}+b)\\\frac{ \partial z }{ \partial x } =2x(y^{2}+b)=p(y^{2}+b)\\y^{2}+b=\frac{p}{2x}\\ \\\frac{ \partial z }{ \partial y } =2y(x^{2}+a)=q(x^{2}+a)\\x^{2}+a=\frac{q}{2y} \\ \\ z=\frac{pq}{4xy}\\ pq=4xyz
\end{aligned}
$$

**For the PDE for all sphere of radius r having center in the $xy$ plane** 

Equationof sphere is $$(x-a)^{2}+(y-b)^{2}+(z-c)^{2}=R^{2}$$ if centered on $xy$ plane, then we get $c=0$, $$(x-a)^{2}+(y-b)^{2}+z^{2}=R^{2}$$
diff partially wrt $x$ $$2(x-a)+2z\frac{ \partial z }{ \partial x }=2(x-a)+2zp =0$$
diff wrt $y$ $$2(y-b)+2z\frac{ \partial z }{ \partial y }=2(y-b)+2zq =0$$
we get 
$$
\begin{aligned}
y-b=-zq \quad\&\quad x-a=-zp\\z^{2}p^{2}+z^{2}q^{2}+z^{2}=R^{2}\\\fbox{$z^{2}(p^{2}+q^{2}+1)=R^{2}$}
\end{aligned}
$$

## By eliminating arbitrary functions 
Form the PDE by eliminating arbitrary functions for the following. 

$z=F(x^{2}+y^{2})$
Diff wrt $x$ $$\frac{ \partial z }{ \partial x }  =\frac{ \partial F }{ \partial x } 2x=p$$
and wrt $y$ $$\frac{ \partial z }{ \partial y } =\frac{ \partial F }{ \partial y } 2y=q$$

# Lagrange multiplier method



--- 
# Charpits method 

## type1 Equations containing $p,q$ only

idk wtf is going on, refer lab manual. 

**Solve** $p^{2}+q^{2}=m^{2}$ 

1. Assume $z=ax+by+c$ is solution
2. put $p=\frac{ \partial z }{ \partial x }=a$
   put $q=\frac{ \partial z }{ \partial y }=b$
   in the question 

   $$ \begin{aligned} a^{2}+b^{2}&=m^{2}\\ b&=\pm\sqrt{  m^{2}-a^{2}}\\\implies z&=ax\pm\sqrt{ m^{2}-a^{2} }+c \end{aligned}$$

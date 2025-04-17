

UNIT I:
Crystal structure-Unit cell and its characteristics, seven crystal systems, and
Bravais- lattices. Symmetry elements in crystals - cubic crystal. Miller indices, Inter
planar spacing, Lattice directions, planes. Wigner - Seitz cell, Concept of reciprocal
lattice point, calculation of reciprocal lattice point of SC, BCC and FCC lattices. Lattice
directions and planes using miller indices. Structure of first Brillouin zone. Geometric
structure factor. Atomic form factor

SO, 
Solids : 
1. Crystalline 
   - Short range order 
   - distinct melting point
   - Anisotropic - direction dependent
   - 
2. Amorphous
   - Short range order
   - has a range of melting temp 
   - Isotropic - direction independent 

# Crystals
   can be of two types : 
   1. Single crystal ![[Pasted image 20241205123541.png]]
   2. Polycrystalls 
![[Pasted image 20241205123252.png]]

# Lattices 
A lattice a set or array of points when environment of each point is identical. Periodic placement of points
a lattice s 2D or 3D, 
Incase of a 2D lattice - one can consider points at distance $a$ along one direction and $b$ along other, the coordinate of any point can be expressed as $\vec{R}=n_{1}\vec{a}+n_{2}\vec{b}$ 
similarly for 3D lattice with $3rd$ basis $\vec{c}$ giving $\vec{R}=n_{1}\vec{a}+n_{2}\vec{b}+n_{3}\vec{c}$ 

types include :
1. Cubic $a=b=c$ $\alpha=\beta=\gamma=90$
2. Tetragonal $a=b\neq c$ $\alpha=\beta=\gamma=90$
3. Orthorhombic $a \neq b\neq c$ $\alpha=\beta=\gamma=90$
4. Trigonal/Rhombic $a=b=c$ $\alpha = \beta = \gamma \neq 90$
5. Hexagonal $a=b\neq c$ $\alpha=\beta=90, \gamma=120$
6. Monoclinic $a \neq b\neq c$ $\alpha=\gamma=90,\beta \neq 90$
7. Triclinic $a \neq b\neq c$ $\alpha \neq \gamma \neq \beta \neq 90$ 

- In cubic - we have face centered and body centered unit cells 
- tetragonal Body centered
- In orthorhombic we have body, face and end centered
- In monoclinic we have base centered 
Giving us 14 **Bravis Lattices** 

We have 5 types of cells 
If unit cell represents only one lattice point, then it is a primitive unit cell. such as E and C

# Unit cell parameters

|                       | Simple cubic Cell        | Body Centered Cell         | Face Centered Cell                             |
| --------------------- | ------------------------ | -------------------------- | ---------------------------------------------- |
| No. of lattice points | $\frac{1}{8}\times{8}=1$ | $\frac{1}{8}\times{8}+1=2$ | $\frac{1}{8}\times{8}+ \frac{1}{2}\times{6}=4$ |
| Coordination no.      | 6                        | 8                          | 12                                             |
| Edge length vs radius | $a=2r$                   | $a=\frac{4r}{\sqrt{ 3 }}$  | $a=2\sqrt{ 2 }r$                               |
| Packing density       |                          |                            |                                                |
# Relation between density and 

$$
\begin{aligned}
\rho=\frac{m}{v}=\frac{n\left( \frac{A}{N_{A}} \right)}{a^{3}}\\\implies \fbox{$a^{3}=\frac{nA}{N_{A}\rho}$}
\end{aligned}
$$

# Symmetry Elements

Symmetry operation - Operations that the system is invariant to (rotation, translation etc.)

### Translational symmetry 
$$x=x+T$$ where $T$ is the edge length. 

### Rotational Symmetry
$$ \theta=\theta+\phi $$
Diad axis - symmetry at 180 deg 
Triad axis - symmetry at 120 deg 
Tetrad axis - symmetry at 90 deg 

Pentad fails because of [[Hausdorf covering]] 
### Reflection Symmetry 

### Inversion symmetry 
Symmetric around center of symmetry 

>[!tip] Crystalls without center of symmetry have piezoelectric property ?

https://www.youtube.com/watch%3Fv%3DwcJXA8IqYl8&ved=2ahUKEwicvajz1KGKAxWx4jgGHYJXNgEQwqsBegQIDRAF&usg=AOvVaw3jnjof8lFx4GBtqaL5wYGN

## Symmetry in a  Simple cube 

Rotational symmetry for a cubic structure.
Diad axis - symmetry at 180 deg 6 axis - 2 fold symmetry
Triad axis - symmetry at 120 deg 4 axis - 3 fold symmetry
Tetrad axis - symmetry at 90 deg 3 axis - 4 fold symmetry

thus it has 13 axis of symmetry 
1 center of symmetry 
![[Pasted image 20241212125342.png]]



what ??

*** 
# Relation between interplanar distance and edge length
![[Pasted image 20250113122032.png]]

$$
\begin{aligned}
OP=&d_{HKL}\\
\begin{matrix}
OA = \frac{a}{h} &\cos\alpha=\frac{OP}{OA}&=\frac{d_{hkl}}{\frac{a}{h}} \\
OB = \frac{b}{k} &\cos\alpha=\frac{OP}{OB}&=\frac{d_{hkl}}{\frac{b}{k}} \\
OC = \frac{c}{l} &\cos\alpha=\frac{OP}{OC}&=\frac{d_{hkl}}{\frac{c}{l}}
\end{matrix}\\
d_{hkl}=\frac{a}{\sqrt{  h^{2}+k^{2}+l^{2}}}
\end{aligned}
$$
$$d^{2}_{hkl}\left[ \frac{h^{2}}{a^{2}}+\frac{k^{2}}{b^{2}}+\frac{l^{2}}{c^{2}} \right]=1$$
**Nickel crystal has FCC structure and has atomic radius $0.1278 nm$. Calculate the interplanar spacing for $(3,2,1)$ plane** 
$r=\frac{\sqrt{ 2 }}{4}a$ 
thus $a=3.614 Ang$ thus the interplanar distance is $d_{hkl}=\frac{a}{\sqrt{  h^{2}+k^{2}+l^{2}}}=\frac{3.61}{\sqrt{  3^{2}+3^{2}+1^{2}}}=0.9Ang$ 

**Interplanar spacing of $110$ is 2 ang. find atomic radius if structure is body centered.**
$$
\begin{aligned}
a=d\sqrt{ h^{2}+k^{2}+l^{2} }
1.2247
\end{aligned}
$$
**A lattice has FCC has lattice constant - 3.52 ang.. calculate interplanar spacing of 101, 123, 320 planes** 

$$
\begin{aligned}
d=\frac{3.52}{\sqrt{ 1^{2}+0^{2}+1^{2} }}=\frac{3.52}{\sqrt{ 2 }} ang\\
d=\frac{3.52}{\sqrt{ 1^{2}+2^{2}+3^{2} }}=\frac{3.52}{\sqrt{ 14 }} ang\\
d=\frac{3.52}{\sqrt{ 3^{2}+2^{2}+0^{2} }}=\frac{3.52}{\sqrt{ 13 }} ang
\end{aligned}
$$
# Wigner Seitz cell
![[Pasted image 20250113123118.png]]
It is a volume surrounding a lattice point which is closer to this cell than any other Lattice Point 

Useful for Brillouin lattice? and xray diffraction 

>[!NOTE] Lattice points + basis gives us crystal
>

# Reciprocal lattice

From [[Bragg's Law]] we take $\sin\theta=\frac{n\lambda}{2d}$ ? 

$$
\begin{matrix}
\vec{a}&\vec{a^*}=2\pi \frac{\vec{b} \times \vec{c}}{V} \\
\vec{b}&\vec{b^*}=2\pi \frac{\vec{c} \times \vec{a}}{V} \\
\vec{c}&\vec{c^*}=2\pi \frac{\vec{a} \times \vec{b}}{V}
\end{matrix}
$$
And also 
$$
\begin{aligned}
V=&\vec{a}\cdot(\vec{b} \times \vec{c})\\
=&\vec{b}\cdot(\vec{c} \times \vec{a})\\
=&\vec{c}\cdot(\vec{b} \times \vec{a})
\end{aligned}
$$

The reciprocal vectors are perpendicular to the other two vectors 
A reciprocal lattice will be having a point which represents a set of planes. (every point represents a set of planes)

Distance between two points is inversely proportional to the interplanar distance

The reciprocal of the reciprocal lattice is the real lattice. 

The reciprocal of simple cubic is smoll simple cubic cell

Now, for Body centered cell, 
![[Pasted image 20250118111848.png]]

$$
\begin{matrix}
\vec{a} & \frac{a}{2}(\hat{\mathbf{x}}+\hat{\mathbf{y}}-\hat{\mathbf{z}}) \\
\vec{b} & \frac{a}{2}(-\hat{\mathbf{x}}+\hat{\mathbf{y}}+\hat{\mathbf{z}}) \\
\vec{c} & \frac{a}{2}(\hat{\mathbf{x}}-\hat{\mathbf{y}}+\hat{\mathbf{z}})
\end{matrix}
$$

Now computing $\vec{b} \times \vec{c}$ 
$$
\begin{aligned}
 \frac{a}{2}(-\hat{\mathbf{x}}+\hat{\mathbf{y}}+\hat{\mathbf{z}}) \times \frac{a}{2}(\hat{\mathbf{x}}-\hat{\mathbf{y}}+\hat{\mathbf{z}})\\=\frac{a^{2}}{4}[\hat{\mathbf{x}}+\hat{\mathbf{y}}] 
\end{aligned}
$$
but $V=\vec{a}\cdot \vec{b} \times \vec{c}$ 
$$
\begin{aligned}
\frac{a}{2}(\hat{\mathbf{x}}+\hat{\mathbf{y}}-\hat{\mathbf{z}}) \cdot \frac{a^{2}}{4}[\hat{\mathbf{x}}+\hat{\mathbf{y}}]\\=\frac{a^{3}}{2}
\end{aligned}
$$
and
$$
\begin{aligned}
\vec{a}^* = \frac{2\pi (\vec{b} \times \vec{c})}{V}\\ \\ =\frac{2\pi \frac{a^{2}}{4}[\hat{\mathbf{x}}+\hat{\mathbf{y}}]}{\frac{a^{3}}{2}}\\=\frac{\pi}{2a}(\hat{\mathbf{x}}+\hat{\mathbf{y}})
\end{aligned}
$$
Now, for Face centered cell
![[Pasted image 20250118113730.png]]

$$
\begin{matrix}
\vec{a} & \frac{a}{2}(\hat{\mathbf{x}}+\hat{\mathbf{y}}) \\
\vec{b} & \frac{a}{2}(\hat{\mathbf{y}}+\hat{\mathbf{z}}) \\
\vec{c} & \frac{a}{2}(\hat{\mathbf{x}}+\hat{\mathbf{z}})
\end{matrix}
$$
giving us, 


>[!tip] Brullouin Zone 
>Wigner Seitz cell of a reciprocal lattice

[[X- rays]] [[Bragg's Law]] 
[[Von Laue Condition]]  

# Classical free electron theory of metals 

micro theory of electrons with mobility etc

The classical theory failed because it failed to explain why multivalent metals were not ore conductive. 

# Sommerfield Quantum free electron theory 

![[schro.jpg]] 

Refer the schrodinger equation

Consider a solid cubic element. we can treat this as a 3D potential well, 
Step 1. Setup the equation for 1D $$\frac{ \partial^{2} \Psi }{ \partial x ^{2} } +\frac{2mE}{\hbar ^{2}}\Psi(x)=0$$
and we know that $E=\frac{mv^{2}}{2}$ and so $2mE=m^{2}v^{2}=P_{x}^{2}$ (momentum square along $x$) 
and we know $p=\hbar k$ and $E=\hbar \omega$ 
$$
\frac{ \partial^{2} \Psi }{ \partial x ^{2} } +k^{2}_{x}\Psi(x)=0
$$
solving which gives $$\Psi(x)=Ae^{ik_{x}x}$$ similarly, the triplet for 3 dimensions are 
$$
\begin{matrix}
\Psi(x) & Ae^{ik_{x}x} \\
\Psi(y)&Ae^{ik_{y}y} \\
\Psi(z)&Ae^{ik_{z}z}
\end{matrix}
$$
giving us 
$$
\Psi(x,y,z)=Ae^{i(k_{x}x+k_{y}y+k_{z}z)}
$$
Implying $k=\sqrt{ k^{2}_{x}+k^{2}_{y}+k^{2}_{z} }$ 
### Fermi energy level 
All energy levels below are occuplied and above is empty 
# Fermi energy vector 

Fermi Energy Sphere

Velocity of electron is fermi velocity 

# Density of states 

Failures of quatum free electron theory
1. Could not explain Band gap 
2. Lattice potential
3. Variation of conductivity with temperature
4. Not explain conductivity due to positive charges (holes in semiconductos
5. Positive hall coeffs

# Bloch theorem

# Kronig Penny model 

Similar to the potential well buisnes but we have $V(x)=V(x+a+b)$ where $a$ is thickness of well, $b$ is thickness of the 'step' in this squarewave like graph. 
We somehow get 
$$
\frac{\beta^{2}-\alpha^{2}}{2\alpha\beta} \sin(\alpha a)\sinh(\beta b)+\cos(\beta b)\cosh(\beta b)=\cos(k(a+b))
$$
heh ? 

Determine position of Fermi level in an intrinsic conductor from the center of the forbidden gap at room temp if the effective mass of electron is twice the effective mass of hole



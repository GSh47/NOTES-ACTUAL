## Assumptions
- Free electrons behave like gases, obeying Maxwell-Boltzmann Statistics.
- Electrons in a conductor travel in all possible directions with all possible velocities(That is, there is no bias to a specific direction or velocity unless an external field is introduced). Thus there is no net current in the absence of an external field. Electrons, thus, also have a Thermal Velocity(in accordance with Maxwell-Boltzmann distribution) of $v_{TH}=\sqrt{\frac{3K_BT}{m_e}}$ , that is proportional to $\sqrt T$, in 3D space. 
- Electron-Electron and Electron-ion interactions can be neglected.
- Electron-Positive ion collision causes resistance, and the behaviour of these particles before and after collisions follow Newtonian laws.(Drude Model)
- Heat is also conducted by these free electrons since they are the only mobile particles in a conductor. Their behaviour can be modelled using Kinetic theory of Ideal Gases.(Lorentz-Drude Model)

## Expression for Electrical Conductivity($\sigma$)

#lookhere Fig(1)

Let us take a Conductor with $n$ electrons per unit Volume. On exposing this conductor to an Electric field of $E$, the force acting on each of it's electrons in $e\times E$, since by Coulomb's Law:$$F=\frac 1 {4\pi\epsilon_0}\frac{Q}{r^2}q=qE$$
where $q=+e$ in the case of a positive test charge.
Since we assume Newtonian interactions, we have:$$F=ma=eE\tag{1}$$Using this, we need to find an expression for Electric Current($I$) to compute the conductivity($\sigma$).

Approach: 
1) We can do this by first finding the drift velocity($v_D$, again following Newtonian Uniform acceleration equation: $v=u+at$ where $at$ is the drift velocity due to acceleration $a$) of an electron.
2) Computing the net flow of all electrons, which is Current. 
3) Compute Conductivity using the expression $J=\frac I A=\sigma E$(Ohm's law in Vector form). This can also be done using the scalar form of the equation $V=IR$, where $E=\frac V L$ and $\sigma=\frac L {RA}$.

 Hence, we have drift velocity $v_D=a\tau$ where $\tau$ is the average time period between two successive electron-positive charge collision(Because on collision, velocity temporarily becomes zero, after which electrons are diverted to conserve momentum, and again accelerated with a drift due to the Electric field).  Therefore, from $(1)$:$$ma=eE\implies ma\times\tau=eE\times\tau\implies m\times v_D=eE\tau\implies v_D=\frac{eE\tau}m\tag{2}$$
Thus, for a cross sectional area of $A$, a Volume of $Av_D$ is swept by the electrons per unit time (like water flowing through a hose pipe). Hence, in our conductor with electron density $n$, number of electrons flowing per unit time is $n\times Av_D$, and subsequently, since each particle possesses a charge of $e$, charge flowing per unit time is $$e\times nAv_D=I\tag{3}$$
Using the Vector representation of Ohm's law, we have from $(3)$:$$J=\frac I A=\frac{enAv_D}{A}=env_D=\sigma E\tag{4}$$
But from $(2)$, we have an equation relating $v_D$ and $E$. Therefore from $(2)$ and $(4)$:$$\sigma E=en\times (\frac{eE\tau}m)=\frac{ne^2\tau}mE$$$$\implies\sigma=\frac{ne^2\tau}m\tag{5A}$$
(Also known as Drude's Equation)

Note that $v_{TH}=\frac\lambda\tau\implies \tau=\frac \lambda {v_{TH}}$  where $\lambda$ is the mean free path. Hence (5) can be rewritten as:$$\sigma=\frac{ne^2\lambda}{mv_{TH}}\tag{5B}$$

In both cases, $\frac {e\tau}m=\frac{e\lambda}{mv_D}=\mu$ is taken as the Mobility of electrons in this medium.$$\implies\sigma=ne\mu\tag{5C}$$

## Expression for Thermal Conductivity($K$)

#lookhere Fig(2)

Consider a rod placed along X-axis having an area of cross section A and heated at one end($x=0$), with number of free electrons per unit Volume $n$. Let the rate of heat conducted per unit time be $\dot{Q}$. Since heat energy is conducted from a hot region to the cold region, $\dot{Q}$ depends on the temperature gradient along the rod($\nabla T$ or simply $\frac{dT}{dx}$ in 1D, i.e. along X-Axis). It also depends upon the area of cross section($A$) of the conductor. Therefore, we have:$$\dot{Q}\propto A\frac{dT}{dx}$$
Thus, for a given time interval $t$, we have heat transferred in time $t$(for a time independant $A$ and $\frac{dT}{dx}$):$$Q\propto A\frac{dT}{dx}\times t\implies Q=K_{TH}\times A\frac{dT}{dx}t\tag{6}$$
Where $Q$ is the Net heat that has been conducted in time $t$, and $K_{TH}$ is the thermal conductivity of the material(behaves as the proportionality constant here).
We now need to find an expression for $K_{TH}$. We can do so using Kinetic Theory of Gases.

Approach:
1) Find an expression for number of electrons travelling the conductor per unit time in terms of the Thermal Velocity($v_{TH}$)
2) Hence, Relate the Kinetic energy of each particle($\frac12 mv_{TH}^2$) to Energy transferred per unit time per unit area, given in $(6)$, to get an expression for $K_{TH}$. 

Let us hence to look at the Energy transferred between two points $E$ and $F$ on the conductor, seperated by a distance of $2\lambda$(twice the mean free path), as shown in the figure. Let $T_1$ and $T_2$ be the steady temperatures and $E$ and $F$ respectively, maintained by the heat source at $x=0$.

Since the temperature gradient is negative, $\implies T_1>T_2$, and therefore Heat flows from $E$ to $F$. Again, since there is no bias towards a particular direction until an external field is introduced, Number of electrons travelling along a particle along each direction is equal along all six directions($\pm X,\pm Y, \pm Z$). Thus number of electrons, per unit volume, travelling along any one of these directions is $\frac n6$. 
Hence, the number of electrons travelling per unit cross-sectional area per unit time is:$\frac n6\times v_{TH}$.
Thus, the number of electrons travelling in time $t$ for cross-sectional area $A$ is: $$\frac {nv_{TH}}6\times t\times A\tag{7}$$
Since only electrons travelling along $\pm X$ contribute to conduction, we only need to find the net $Q$ from $E$ to $F$.
The Energy possessed by each particle is $\frac 32 k_BT$. Hence, Energy transferred from $E$ to $F$ is:$Q_{EF}=\frac 32 k_BT_1\times \frac {nv_{T_H}}6At$ and similarly Energy transferred from $F$ to $E$ is: $Q_{FE}=\frac 32 k_BT_2\times \frac {nv_{T_H}}6At$.
Thus net $Q$ along $EF$ is:$$Q=Q_{EF}-Q_{FE}=\frac {\cancel3}2 k_BT_1\times \frac {nv_{T_H}}{\cancel{6}2}At-\frac {\cancel3}2 k_BT_2\times \frac {nv_{TH}}{\cancel{6}2}At=\frac{k_Bnv_{TH}}{4}\times At\times (T_1-T_2)\tag{8}$$
Therefore, from $(6)$ and $(8)$, we have:$$K_{TH}\times \cancel A\frac{dT}{dx}\cancel t=\frac{k_Bnv_{TH}}{4}\times \cancel{At}\times (T_1-T_2)$$where $\frac{dT}{dx}=\frac{T_1-T_2}{2\lambda}$ for the discrete points, E and F. Hence:$$K_{TH}{\frac{\cancel{T_1-T_2}}{\cancel 2\lambda}}=\frac{k_Bnv_{TH}}{\cancel 4 2}\times \cancel{(T_1-T_2)}\implies K_{TH}=\frac{k_Bnv_{TH}\times \lambda}{2}\tag{9}$$
## Wiedemann-Franz Law:
(Relation between $\sigma$ and $K$)

Dividing $(9)$ with $(5B)$, and using $(2)$ we get the ratio between Thermal and Electrical Conductivity:$$\frac {K_{TH}}\sigma=\frac{k_B\cancel{n}v_{TH}\cancel\lambda}{2}\div \frac{\cancel{n}e^2\cancel\lambda}{mv_{TH}}=\frac{k_Bv_{TH}^2m}{2e^2}$$
But $\frac 12 mv_{TH}^2=\frac 32 k_BT$. Therefore:$$\frac {K_{TH}}\sigma=\frac{k_B}{e^{2}}\times\frac 32 k_BT=\frac32 (\frac{k_B}{e})^{2}T\propto T\tag(10)$$

That is, the ratio of thermal conductivity and electrical conductivity at a particular temperature T is same for all metals. This is known as Wiedemann – Franz Law. i.e.:$$\frac {K_{TH}}{\sigma T}=\frac32 (\frac{k_B}{e})^{2}=L$$ where $L$ is known as the Lorentz number.
Thus, all good conductors of heat are also good conductors of electricity.
## Drawbacks of Classical Theory


1) According to Lorentz-Drude relation (5B), $\sigma\propto \frac{1}{\sqrt T}$, but experiments showed that $\sigma\propto \frac{1}{T}$.
2) From $(5A)$, $\sigma\propto n$, but this was found to not always be true.
3) Lorentz number's experimental value was found to be different
4) Theory could'nt explain why some materials were conductors while others were'nt.
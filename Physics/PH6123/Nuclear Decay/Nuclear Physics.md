![[Nuclear Physics 2025-03-09 16.13.34.excalidraw]]
- Note on [Rydberg atoms](https://www.google.com/url?sa=t&source=web&rct=j&opi=89978449&url=https://en.wikipedia.org/wiki/Rydberg_atom&ved=2ahUKEwiHm5qe6o-KAxVMjGMGHYTrFrkQFnoECBwQAw&usg=AOvVaw0Gd8FHTFpOB7HYFCjp-WoH) 
- Line defects and molecular what placing aoms in uni cells

Order of sizes : Atoms - $1\sim 10 A^{\circ}$  while nucleus is $\sim 10^{-15}$ Fermi 

Notation : $$_{1}^{1}p\quad ^1_{0}n\quad _{-1}^1e$$
subscript is charge and superscript is number of nucleons in the entity  

Rule of thumb - the object must be a quarter of the interacting wavelength. 

Find mass of electron in energy units, $\frac{m_{e}c^{2}}{e}\to 0.5$MeV !

1. Made up of neutrons and protons
2. Rutherford in scattering experiments observed that $\alpha$ particles ($^4_{2}He$) approach teh nucleus to a distance of $\sim 3\times 10^{-15}m$ 
3. Nucleus does not have a definite sharp boundary
4. Nucleus is modeled as a sphere of posititve charge. but since there is no definite boundary - if we perform a scattering experiment with electrons then we will see a range of cross sections and the average is considered.

# Properties 
Nuclear density $\rho=\frac{ \text{Atomic mass Z}}{\text{Volume V}} \sim const.$ 
implies $V\propto Z$
$$
\begin{aligned}
V=kZ\\ \frac{4}{3}\pi r^{3}=kZ\\\implies r=KZ^{1/3}
\end{aligned}
$$
THe mass is assumed to be uniformly distributed throughout nuclear volume. therefore uclear charge densitty is approx a constant throughout the nuclear volume. 
Implies distribution of nuclear charge follows the saame pattern as mass distribution. 
Implies radius can also be measured on the basis of nuclear charge. This is called charge radius of the nucleus. 

Experimentally nuclear size can be estimated in two ways. 
1. Nuclear force method 
   Based on range of nuclear forces and is probed by scattering method
   Example : Rutherford $\alpha$ scattering, isotope shift in line spectra, $\alpha$ decay etc.  
2. Electrical method
   Based on Electric field, charge distribution, 
   Example - electron scattering, mirror nuclei method, muonic xray method. 
# Mirror nuclei method 

> Mirror nuclei has the same number of nucleons but the number of protons in one nucleus is going to be equal to the number of neutrons in the other nucleus. 
> Example $^{11}_{6}C:^{11}_{6}B$


Existence of protons in the nuclei gives rise to coulomb repulsive forces and hence nuclear coulomb energy 
Let $\rho=$ charge density. $\frac{Ze}{\frac{4}{3}\pi r^{3}}$
Assume that at one instant of time - we have a spherical ball of radius $x$
 This implies charge $q_{1}$ of the sphere is going to be equal to $\rho \times\frac{4}{3}\pi x^{3}$ 
 The ball is surrounded by sphereical shell of thickness $dx$ and radius $x$. The charge inside the shell is $q_{2}=\rho \cdot{4}\pi x^{2}dx$ 
 Implies that the total potential energy $d\cdot E_e=\frac{1}{4\pi\epsilon_{0}}\left( \frac{q_{1}q_{2}}{x} \right)$ 
 $$
\begin{aligned}
E_{e}\int   \, dx 
\end{aligned}
$$
for **two adjacent mirror nuclei** (differ by $Z=1$) having charges $Ze$ and $(Z+1)e$ but having same radius $R$ 
$$
\begin{aligned}
\Delta E_{c}=\frac{1}{4\pi\epsilon_{0}} \frac{3}{5} \frac{1}{R} ((Z+1)^{2}-Z^{2})e^{2}
\\=\frac{1}{4\pi\epsilon_{0}} \frac{3}{5} \frac{1}{R} e^{2}(2Z+1)
\end{aligned}
$$
now $2Z+1=A$ which is atomic mass. giving us 
$$
\frac{1}{4\pi\epsilon_{0}} \frac{3}{5} \frac{e^{2}}{R} A
$$
example: 

$$R=\frac{1}{4\pi\epsilon_{0}} \frac{3}{5} \frac{e^{2}}{\Delta E_{c}}A$$  
given two atoms $$^{29}_{14}Si,^{29}_{15}P$$ 
When we are estimating the nuclear radius using the formula $R=R_{0}A^{1/3}$ we are assuming that **nuclear mass density is constant**  and hence we are estimation the mass distribution radius of the nucleus. 

When using $\Delta E_{c}$ formula, we are assuming that **nuclear charge is distributed uniformly** and we estimate the nuclear charge radius

## important data 

$$
\begin{matrix}
electron & m_{0}c^{2}=511KeV \\
1amu&931 MeV\\hc&1240MeV\cdot fm
\end{matrix}
$$

# Electron scattering method 

Assume that a partially coherent beam of electrons gets scatered from the nucleus. 
Example -  Electrons are scattered from $^{10}O$ further assume that the energy of the incident electrons =$420$ MeV. Under such situation the intensity of the scattered radiation as a function of angle $\theta$ can be estimated and exhibits a graph as shown below. 
![[Nuclear Physics 2024-12-19 10.44.07.excalidraw]]

1. If the incident electron is scattered from the electrons bound to the atom, then electrons have very less energy. this implies we can use electronic circuitry to veto such electrons. 
2. If incident electrons are scattered from a heavy nucleus then it's energy will be very high as very little energy is transferred to the nucleus. 
3. Rough calculation ; 
   Treat the nucleus as a circular aperture
   treat electrons as coherent waves incident on aperture
under these assumptions, from optics - we can see that $$I=\text{intensity of scattered electrons}\left(  \frac{\sin^{2}(\beta)}{\beta^{2}} \right)$$ 
the brcket term is 'sinc squared function' and $\beta=\frac{\pi}{\lambda}D\sin\theta$ (path diff ?) and we see that $I=0$ when $D\sin\theta=\lambda,2\lambda\dots$ or $\sin\theta \sim 1.22\frac{\lambda}{D}$ 

If we make the nucleus analogus to the circular disk, and noting that  from the diffraction pattern from oxygen - minima happens when $\theta$ is around 45 deg, then we get 
$$
\begin{aligned}
\sin43=1.22 {\frac{\lambda}{ D}}
\end{aligned}
$$
can we get the second minima from oxygen 10 nucleus ?

# Determination of nuclear mass using mass spectrometer. 

![[Pasted image 20250109101024.png]]


## ion source
- produces beam of ionised atoms or molecules that 
- often a vapour of the material being studied is ionise by bombarding with electrons or spark discharge coated with material under study
- ions emerging from the ion source will have range of velocities and a range of masses 
## Velocity selector 
- Here we allow ions having one particular velocity to go out of this cahmber 
- THis is achieved by using mutually perpendicular $\vec{E},\vec{B}$ 
	- $\vec{E}$ tries to deflect the ions in the upward direction as per the formula $$\vec{F}=q\vec{E}$$
	- $\vec{B}$ tries to deflect the particle downwards as per the formula $$\vec{F}_{B}=q(\vec{v}\times \vec{B})$$
	- We select only those ions of particular velocity correspoding to $$qE=qvB$$$$\therefore v= \frac{E}{B}$$
## Momentum selector, 
These selected ions are sent to momentum selector, where the $\vec{B}$ is directed opposite to the $\vec{B}$ in velocity selector
In this region we have the particles bent in a uniform $\vec{B}$ field. 
$$
\begin{aligned}
\frac{mv^{2}}{r}&=qvB\\
m&=\frac{qBr}{v} =\frac{qBr}{\left( \frac{E}{B} \right)}\\m&=\frac{qB^{2}}{E}r
\end{aligned}
$$
Note : Due to sensitivity issues we usually try to find those atoms and molecules with low  masses with 
 
# Nuclear shape 
When we use the equation $r=r_{0}A^{1/3}$ we assume that the nucleus is a sphere. 
Many nuclei has however an intrinsic quadrupole moment in addition to magnetic moment. This is due to elliptical distribution of charge inside the nucleus. $q=\frac{1}{2}(3z^{2}-r^{2})$ where $r$ is the avg radius (avg of semi minor and semi major axis) of nucleus and $z$ = spin axis.   
- Nuclear quadrupole moment is possible only when the total angular momentum or nuclear spin or isospin $(I)\geq 1$ 
- Depending upon the nuclear shape, with referfence to the spin axis, the nucleus can be called as either prolate or oblate depending on whether $q=\frac{1}{2}(3z^{2}-r^{2})$ is positive prolate or negative oblate. 

# Nuclear forces
Properties : 
1. Nuclear forces are strongly attractive. They are ususally $10^{21}$ stronger than electrostatic forces
2. Nuclear forces are charge independent forces, 
3. They are short range forces, typically dies down rapidly after a distance of few fermis
4. They are saturated forces. Implies binding energy per nucleon in approx a constant. implies each nucleon interacts only with a limited number of other nucleons. 
5. Nuclear forces are spin dependent forces. 
6. At extremely short distances $\sim 0.4F$ they are repulsive. ![[Nuclear Physics 2025-01-16 10.39.57.excalidraw]]
## Yukawa's theory of exchange forces to explain nuclear forces :
According to yukawa, the nuclear forces between nucleon arise due to exchange particles called muon $\mu-$meson having mass $\sim 200m_{e}$.
later it was discovered that it is due to $\pi-$meson exchange and there are 3 different types of $\pi-$mesons, $\pi^0,\pi^+,\pi^-$ 
1. $\pi^+$ exchanged between proton-proton
2. $\pi^-$ is exchanged between proton-neutron
3. $\pi^0$ is exchanged between neutron-neutron

McKenzie economic trnadss

- [ ] Radiocarbon dating LIMITATIONS
Only for organics upto about 55000 years ago 

# Theory of succesive disintegration.
In nuclear decay, parent always decays into a daughter nucleus $A\to B\to C$ which inturn decays into grandaughter till a stable nucleus is obtained. Example : Uranium series, Actinium series, Thorium series. (Find the decay scheme for one or two of them ). 
The number of parent atoms at time $t=0$ is $N_{0}$
The number of parent atoms at time $t=t$ is $N_{1}$
The number of daughter atoms at time $t=t$ is $N'$ 
and so on, 
THis implies - rate of disintegration of parent element is given bythe formula $\frac{dN_{1}}{dt}=-\lambda_{1}N_{1}$ 
this implies rate of formation of the daughter  nuclei is $\lambda_{1}N$ 
rate of disintegration of daughter nucleus is $\lambda_{2}N'$ 
Therefore net rate of formation of granddaughter nuclei is given by $\frac{dN'}{dt}=\lambda_{1}N_{1}-\lambda_{2}N'$ 
therefore the equation is given by $\frac{dN'}{dt}+\lambda_{2}N'=\lambda_{1}N_{0} e^{-\lambda_{1}t}$ 
this gives us $$\frac{dN_{2}}{dt}e^{\lambda_{2}t}+\lambda_{2}N_{2}e^{(\lambda_{2}t}=\lambda_{1}N_{0}e^{(\lambda_{2}-\lambda_{1})t}$$ Integrate to get $$N_{2}e^\lambda_{2}t=\frac{\lambda_{1}}{(\lambda_{2}-\lambda_{1})}N_{0}e^{(\lambda_{2}-\lambda_{1})t}+const$$
At $t=0,N=N_{0}$ 
$$
\begin{aligned}
0=\frac{\lambda_{1}}{(\lambda_{2}-\lambda_{1})}N_{0}+c\\
c=-\frac{\lambda_{1}}{(\lambda_{2}-\lambda_{1})}N_{0}\\

\end{aligned}
$$

Express N2 as some func of $N_{0}$
# Radioactive equilibrium
## Secular or Permanent Equilibrium
In this case we assume that $\lambda_{2}\gg\lambda_{1}$ implies that mean life of parent is much greater than daughter. Implies $\lambda_{2}-\lambda_{1}\approx\lambda_{2}$ similary $e^{-\lambda_{1}t}\sim 1$ is therefore, $N_{2}=N_{0}\frac{\lambda_{1}}{\lambda_{2}}$ after a long time. Nut $N_{0}\approx N$ as lifetime of parent is very large. $N_{2}\approx \frac{\lambda}{\lambda_{2}}$ this implies formation and disintegration of daughter nucleus becomes equal called as secular equilibrium.  
## Transient Equilibrium 
When $\lambda_{2}\geq\lambda_{1}$ implies that the mean life of the parent is not too different from that of the daughter nucleus. 
$e^{-\lambda_{2}t}$ decays faster 
something $$N_{2}=\frac{\lambda_{1}N_{1}}{(\lambda_{2}-\lambda_{1})}$$ this implies both parent and daughter decay at the rate so that $\frac{N_{2}}{N_{1}}=const$ in a Transient Equilibrium. 

$$
^X_{Z}X\to ^{X-4}Y+^4_{2}He
$$
# Range and energy of $\alpha$ particles
Usually the range is dependent on initial energy it is emitted with., nature of radioactive element , gas through which $\alpha$ particles pass through and pressure of the gas
# Geiger Nuttal Law.
Geiger showed that Range $\propto V_{0} ^{3}$ If the initial energy of $\alpha$ particle is in $MeV$, then it is related by $E=(2.08\times{1}0^{14})bE_{0}^{3/2}$ where $b=3.18\times{1}0^{-3}$ . 
It is observd that nuclei with shorter half life $T_{\frac{1}{2}}$ emit $\alpha$ particles with high energies implies there is a relation between rnage and half life of hte nucleus emitting the radiation. 
This law mathematically expressed as $\log(\lambda) =A\log(R)+B$

**Note** te const $A$ has almost same value for all radioactive series but $B$ has different value for different series. 
The value can also be expressed as $\log(\lambda)=\frac{3}{2}A\log(E)+B'$  
Characteristics of $\alpha$ spectrum. It has been observed by use of strong magnetic fields that nuclei emit $\alpha$ particles with different energies within a narrow range. 

Gamov  - alpha beta gamma 

# Beta decay
## Types 
- **Negatron emission** Ordinary beta emission 
  $_{Z}^AX\to _{Z+1}^AY+_{-1}^0e+\bar{\nu_{e}}$
  Example: $_{1}^3H\to_{2}^3He+_{-1}^0e+\bar{\nu_{e}}$
  Energy released in $\beta^-$ process is $Q=[M_{n}(A_{1}Z)-M_{n}(A_{1}ZH)-m_{e}]c^{2}$
- **Positron emisson** 
    $_{Z}^AX\to _{Z-1}^AY+_{1}^0e+\nu_{e}$
  Example: Find one
  B+ emission is possible only when mass of parent is greater than parent by atleast 1.022MeV 
- **Orbital electron capture** 
  When an unstable proton rich nucleus is present with the coulomb barrier prevents emission of a proton. this impliees that the neucleus can becoe stable only by transforming a proton into a neutron by capturing an orbital electron, hence Orbital electron capture
  Sinc the K shell electron that is close to the  nucleus is ususally captured - it is also called K capture. The effective process in this case is 
  $_{1}^1p+_{-1}^0n+\nu_{e}$  sh



Total energy emitted during $\beta$ decay is equal to th mass difference between parent and daughter nuclei which is equal to kinetic energy of $\beta$ particle 

Large portoin of $\beta$ spectrum exhibits continuous energy unlike $\alpha$ particles which show discrete energy

Typical $\beta$ spectrum ahs the following properties. 
1. A continuous spectrum with energies ranging from origin to some maxima, no sharp peaks are seen. 
2. A line spectrum consisting of a numeber of discrete energues namely $c$ on the continuous spectrum

3. X ray and gamma ray from a source shows line spectrum, but $\beta$ is continuous.  
4. Law of conservation of energy and angular momentum seems to violated since the effective reaction is ... each particle has a spin angular momentum$=\frac{1}{2}\hbar$
5. Total spin of $RHS$ and $LHS$, we have non conservation of ang mom
6. Conservation of linear momentum also seems to be violated. 

Solution to the problem :
Pauli postulate that along with $\beta-$ particle, another particle called the anti neutrino is produced to preserve ang mom. Hence reaction should be 

Follows fermi dirac statistics and has half integer spin. 
Along with $\beta^-$ we have a anti-neutrino is emitted, and with $\beta^+$ we have a neutrino

End point energy is shared between the daughter nucleus, beta particle and neutrino. 

$\bar{\nu}$ and $\nu$ differ from each other by a virtue of their spins. 

# Nuclear models

In the absence of detailed theory of nuclear structure, attempts were made to explain experiments with theoretical models. l 

## Shell Theory 

Assumptions : 
1. Each nucleon moves in it's orbit within the nucleus independently of all the other nucleons. 
2. Orbit is determined by potential energy function $V(r)$ 
3. $V(r)$ represents the avg effect of all interactions wiht other nucleons. 
4. $V(r)$ is same for all nucleons
5. Interaction between nucleons is a small perturbation on the interaction between the nucleon and the potential field. 
6. The potential which describes the nuclear attractions as a form between square-well potential $V(r)=-V_{0}$ and an oscillator function $V(r)=-V_{0}+ar^{2}$ where is the distance between nucleon and center of force ? and $a$ is a ??

Two different kinds of particles protons and neutrons have been considered. The pauli's exclusion principle must be applied to both protons and neutrons, implying that no two protons or neutrons can have same two quantum numbers. 

If we look at the harmonic oscillator function, there will be closed cells at $2, 8, 20, 40,70$ but $50, 82, 126$ 
are missing, those shell numbers appear to have no connection with experimental observations. 

Infinite well potential predict closed shells at $2,8,20$ and many other non-magic numbers. $50,82,126$ are again missing. 
THis implies, to get the correct shell numbers we must make another assumption, nucleons energy depends on whether it's spin angular momentum is paralell or anti paralell with its orbital angular momentum (spin-orbit) coupling. 

When this assumption is made, we get closed nucleon shells at $2,8,20,50,82,126$  in agreement with the experimental data. 

Advantages of shell model, 
1. It predicts the totaal angular momenta of nuclei in good agreement with the experiment. Very useful in studying beta decay. 
2. Using shell model, a correlation has been found between nucleon isomerism (existence of longlived excited states) and magic numbers. 
3. Shell model can be used to predict total angular moment, low lying excited states
4. Experimental data for magic moments/numbers and electric quadrupole moments are also been integrated in terms of shell models eg: if proton numbers are magic, then quadrupole moment is eithe zero or very small number. When a new shell begins to form. Quadrupole number is negative as the number of protons in the unfilled shell is increased, Quadrupole numer becomes positive, and is maximum when it's 2/3 filled. 

Drawbacks 
1. The shell model assumes a sphereical shape for the nucleus could not explain 
	1. excited states of even-even nuclei
	2. Magnitude of nuclear quadrupole moments, magnetic moments of some nuclei. 
2. Probability of radioactive transitions. 
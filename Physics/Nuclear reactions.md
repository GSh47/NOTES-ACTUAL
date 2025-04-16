Thomas Kuhn scintific revolution 

Wilhelm Herschel color temps 

Bunsen and Kirchoff discovery of colour 

# Dynamics of nuclear reactions 

The basic scheme for a nuclear reaction is
$$a_{\text{projectile}}+A_{\text{target}}\to B_{\text{recoil}}+b_{ejectile}$$
The expected condition is $a\neq b$ and $A\neq B$. Incase if by chance $a=b;A=B$ then we have a scattering case. 
The nuclei potential is given by 
![[Pasted image 20250211003040.png]]
 minima is at around -88MeV
## Scattering 
here as discussed,  $a=b$ and $A=B$ , we further have two more cases :
### Elastic scattering 
If the same alpha particle is returned with same energy back towards the detector -  then we have elastic scattering
example : $_{0}n^1+_{92}^{238}U\to_{92}^{238}U+_{0}n^1$
### Inelastic scattering
If the energy is transferred to the nuclei, exciting the target nuclei, taking it to a higher state, then we have inelastic scattering. 
the excited nuclei might ejected a proton in return too, seeming similar. 
$_{0}^1n+_{7}^{14}N\to_{6}^{14}C+_{1}^1H\to$ look it up ?
# Types of nuclear reaction 
The difference is time. If wavelength (matter wave) of projectile is comparable to the entire nucleus, we have a compoud nuclear reaction
If wavelength (matter wave) of projectile is comparable to only a nucleus, we have a direct nuclear reaction... $E=\frac{hc}{\lambda}$ so, higher the energy, lower the waveleength.. i.e **Faster nuclei has DNR, Slower has CNR**
## Direct nuclear reaction 
happens around $10^{-22}$ seconds peak anisotropically distributed
-  **Pickup reactions** The projectile picks up a nucleon quickly and leaves
- **Stripping reactions** The projectile drops off a nucleon quickly and leaves
## Compound nuclear reactions 
much slower $10^{-16}$ seconds  is isotropically distributed.. the wave function of the incident nuclei is larger and interacts with several nucleons before leaving

# Q value of nuclear reactions

This is a part **Nuclear Energetics**. Depending on Q value of a reaction, the reaction is either *Endoergic* or *Exoergic*

![[Pasted image 20250130112856.png]]

We can write by conservation of momentum, 
$$
\begin{aligned}
p_{a}=p_{b}\cos\theta+p_{B}\cos \phi\\\implies p_{a}-p_{b}\cos\theta=p_{B}\cos \phi
\end{aligned}
$$
as only $a$ had momentum before collision 
and on the perpendicular axis, since nothing was moving here before : the initial and thus final momentum here is zero 
$$
\begin{aligned}
0=p_{b}\sin\theta-p_{B}\sin \phi \\\implies p_{b}\sin\theta=p_{B}\sin \phi 
\end{aligned}
$$
From which we can say, 
$$
\begin{aligned}
 \left[p_{a}-p_{b}\cos\theta\right]^{2}+[p_{b}\sin\theta]^{2}&=p_{B}^{2}\cos ^{2}\theta+p_{B}^{2}\sin ^{2} \theta\\&=p_{B}^{2} (\cos ^{2}\theta+\sin ^{2}\theta)\\&=p^{2}_{B}
\end{aligned}
$$
Now, the reaction can be described by conservation of energy as 
$$(m_{a}+m_{A})c^{2}+K_{a}=(m_{b}+m_{B})c^{2}+K_{b}+\frac{p_{B}^{2}}{2m_{B}}$$
now, $(m_{a}+m_{A})c^{2}-(m_{b}+m_{B})c^{2}=Q$
Given all this, we do not know $p_{B}$ Hence we eliminate it by combining the above equations. 
$$
\begin{aligned}
(m_{a}+m_{A})c^{2}-(m_{b}+m_{B})c^{2}=&K_{b}-K_{a}+ \frac{p^{2}_{B}}{2m_{B}}\\
\implies Q=&K_{b}-K_{a}+ \frac{\left[p_{a}-p_{b}\cos\theta\right]^{2}+[p_{b}\sin\theta]^{2}}{2m_{B}}\\
=&K_{b}-K_{a}+ \frac{p_{a}^{2}+p_{b}^{2}\cos ^{2}\theta-2p_{a}p_{b}\cos\theta+p_{b}^{2}\sin ^{2}\theta}{2m_{B}}\\
=&K_{b}-K_{a}+ \left[ \frac{p_{a}^{2}}{2M_{B}} \right]+\left[ \frac{p_{b}^{2}}{2M_{B}} \right]-\frac{2p_{a}p_{b}\cos\theta}{2m_{B}}\\
\\&\text{Now remember $p=\sqrt{ 2mK }$}\\ \\
=&K_{b}-K_{a}+ \left[ \frac{2m_{a}K_{a}}{2M_{B}} \right]+\left[ \frac{2m_{b}K_{b}}{2M_{B}} \right]-\frac{2 \sqrt{ 2maKa }\sqrt{ 2m_{b}K_{b} }\cos\theta}{2m_{B}}\\
 \implies Q=&K_{b} \left[ 1+\frac{m_{a}}{m_{B}} \right] -K_{a}\left[ 1-\frac{M_{b}}{M_{B}} \right]-\frac{2\cos\theta}{m_{B}}\sqrt{ (m_{a}K_{a})(m_{b}K_{b})}
\end{aligned}
$$
# Threshold of Nuclear reactions
The minimum Kinetic energy required by the incident particle to bring about the reaction engergically is called threshold energy of reaction $$
E_{Th}=-Q\left[\frac{M_{a+}M_{A}}{M_{A}} \right]
$$
Calculate the Q value of nuclear reaction 

Calculate the energy released in the following rare spontaneous fission reaction : Calculate amount of kinetic energy produced by fission of 1kg of U235 given avg fission reaction of U235 produces 200MeV 
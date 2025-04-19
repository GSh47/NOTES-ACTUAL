In a conductor of Volume $V$, if $N$ electrons exist in the volume, the ground state of the system can be found by computing the energy possessed by a single electron and the scaling it to $N$ electrons, obeying Pauli's exclusion principle(Every wave vector $\vec k$ has 2 allowed electron levels for spin up and down respectively).
Drawing the $k_x$ vs. $k_y$ vs. $k_z$ diagram, we can observe the different Energy Levels or k-states to be spheres of radius $k=\sqrt{k_x^2+k_y^2+k_z^2}$, related to the Energy of the state by the relation:$$E_k=\frac{\hbar^2k^2}{2m}$$
#lookhere 
Starting from the first k-state at $k=0$, we have $E=0$, having 2 electrons. We keep filling all the Electrons this way until the last shell(Fermi sphere) is completely filled. Shells outside this are unoccupied, and the shells inside(with radius lesser than $k_F$ or the Fermi Wave Vector) are fully filled, where the Fermi Energy, or the Energy at the Surface of the Fermi Sphere at $0K$($E_F$) is given by:$$E_f=\frac{\hbar^2k_f^2}{2m}\tag{1}$$
$E_f$ is also the value of Energy upto which all Energy states in a Fermi gas are filled, and above which all are empty at $0K$.
We can find this Energy by first finding the number of Electrons encased by the Fermi shell, and then computing energy possessed per electron.

## Approach
1) Compute the Volume of the Fermi Sphere(Maximum occupied Volume, or $\frac 43 \pi k_f^3$)
2) Compute Volume of the element volume in the k-space($k^3$)
3) Hence, Compute total number of allowed states, which is twice the ratio of 1) and 2).
4) Find $k_f$ in terms of $N$, and hence $E_f$ in terms of $N$

The Volume of the Fermi sphere can also be determined through the relation:$$V=\frac 43 \pi k_f^3\tag{2}$$
But $k$ values are Integral multiples of $\frac{2\pi}{L}\implies$ the minimum non-zero value of $k=\frac{2\pi}L$. Hence, the element volume in k-space is:$$V_{min}=(\frac{2\pi}L)^3\tag{3}$$ 
Therefore number of allowed energy states($N$) is given by:$$N=2\times \frac V {V_{min}}=\cancel 2 \times\frac {\cancel 4}3 \cancel\pi k_{f}^{3}\div(\frac{\cancel {8\pi^3}\cancel2\pi^2}{L^3})=\frac{k_f^3L^3}{3\pi^2}=\frac{Vk_f^2}{3\pi^2}\tag{4}$$
$$\implies k_f=(3\pi^{2}\frac N V)^{\frac 13}\tag{5}$$
Therefore, from $(1)$ and $(5)$, we have:$$E_f=\frac{\hbar^2}{2m}(3\pi^{2}\frac NV)^{\frac 23}=\frac{\hbar^2}{2m}(3\pi^{2}n)^{\frac 23}\tag{6}$$


## Fermi Velocity and Temperature

Fermi velocity($v_f$) is the velocity of electrons at the Fermi surface. Therefore, from the dispersion relation($p=\hbar k$) and $(5)$, we have:$$p_{f}=\hbar k_{f}\implies v_{f}=\frac{\hbar}m k_f=\frac{\hbar}m(3\pi^{2}\frac N V)^{\frac 13}$$

Fermi Temperature($T_f$) is the temperature at which average Thermal energy of teh free electron in a solid becomes equal to the Fermi Energy at $0K$. i.e.:$$k_BT_f=E_{f}\implies T_f=\frac{E_f}{k_B}$$

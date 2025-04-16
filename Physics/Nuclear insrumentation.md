![[nuclearphys.png]]
Arthur Beiser 
Midsem portions : 
- Particle accelerators & Detectors
	- GM Counter
	- ionisation chamber
	- prop counter
- nucllear accelerators
Q value problem
GM counter problem
Cyclotron problems
minima of nuclei diffraction graph
3 parts in paper : A - 2/3x7=14, B=2/3x , C=
Starts off with a brief discussion on atomic structure : *A uniform E field will not result in large angle deflections, hence there must have been a point concentrated mass to make that happen*
# Gas Detector 

Similar to an alcohol cloud chamber, these work the same way, 

The process is quoted from given notes as : 
1. High energy particle collides with molecules in a medium, energy is transferred to the atom/molecule 
2. The energy is absorbed by electrons in outer shell, which is excited and leaves the atom/molecule creating a free electron and an ion
3. A large number of such pairs are created as the high energy particle passes through the medium
4. The electric field within the tube is in such a way that the electrons and ions are attracted to anode and cathode respectively
5.  The potential drop at Load resistor is created by the accumulation of electrons at the electrode.The electrons complete the circuit and get absorbed by the ions again making them neutral thus constituting a pulse 

More energy a particle has, bigger the pulse. 

The pulses recorded depend on :
1. incident radiation
2. Applied voltage

Types of counters are given as follows

- Ionisation counter
- Proportional counter (primary and secondary ionisation)
- Geiger Muller Counter (Townsend Avalanche effect)

These are pretty much the same device but at different voltages as seen below 

![[Pasted Image 20250107111727_504.png]]

### Ionisation region
it's constant across applied voltge but gives different reading for different ionisation energy
### Proportional region

the count increses proportionally with voltage 

### Geiger region
Plateau region - It does not discriminate wrt $\alpha,\beta,\gamma$ 
A single incidence creates a townsend Avalanche leading to saturated pulse 

# Geiger Counter
## Construction
Abridged from shared pdf : 
It consists of the GM tube which is a hollow metallic cylinder and it contains some kind of a gaseous medium - usually a mixture of 90% Ar and 10% alcohol of some kind. This tube is the Cathode, connected to the negative terminal of a high-tension battery $\sim 3000 V$. Along the centre of the cylinder is  the Anode - a tungsten electrode connected to a load resistance connected to the positive terminal of the battery. Connected parallel to the load resistance is the amplifier and/or a pulse counter to determine potential drop that happens across $R_L$ while also measures the amount of current associated with it. The system is also associated with some kind of a counter that can count that number of events over a period of time.

## Working 
summarized by GPT

1. **Radiation Entry & Ionization**
       - An external nuclear particle (alpha, beta, or gamma) enters the GM tube.
    - This particle ionizes the gas inside, creating free electrons and positive ions.
2. **High Voltage Acceleration**
    - A high voltage (1,000–3,000V) is applied across the tube.
    - Free electrons accelerate towards the anode (central electrode).
    - Positive ions move toward the cathode (metallic cylinder wall).
3. **Avalanche Effect (Townsend Avalanche)**
    - Accelerated electrons collide with gas molecules, causing further ionization.
    - This leads to a chain reaction, producing more electrons and ions.
    - The process rapidly multiplies ionization filling the entire tube, resulting in a discharge.
4. **Signal Detection & Counting**
	-  The accumulated electrons reach the anode, completing the circuit.
    - A potential drop is detected across a resistor (RL).
    - The electronic system registers this as one count, indicating radiation detection.
5. **Dead Time**
    - During discharge, the GM tube cannot detect new particles.
    - This recovery phase is called "dead time" (200–400 microseconds).
6. **Recombination & Resetting**
     - Electrons and ions recombine at the electrodes, restoring neutral gas molecules.
    - The GM tube returns to its original state, ready for the next detection.
7. **Quenching (Preventing False Counts)**
    -  Secondary photon emissions may trigger unwanted ionization.
    - To prevent this, quenching agents (e.g., alcohol) absorb excess energy as rotational or vibrational energy
    - This stabilizes the tube and ensures accurate radiation detection.


## Formulas : 

E field in a tube
$$
E=\frac{V_{0}}{r\log_{e}\left( \frac{b}{a} \right)}
$$
Mean free path $\lambda$
$$
\lambda E=V_{IP}
$$
Gas multiplication factor for prop counters 
$$m=\frac{\text{$\sum$ ion pairs collected }}{\text{$\sum$ ion pairs created }}$$ 
[[questions nuke inst]] 


# Cyclotron
A **cyclotron** is a type of particle accelerator that uses a **constant magnetic field** and a **constant-frequency alternating electric field** to accelerate charged particles in a **spiral trajectory**. 
$$
\begin{aligned}
F=&qvB\\ \frac{mv^{2}}{R}=& qvB\\ t=\frac{2\pi R}{v} \implies &f= \frac{v}{2\pi R} \\ \\f=& \frac{\left( \frac{qBR}{m} \right)}{2\pi R}\\ \\ \fbox{$f=\frac{qB}{2\pi m}$}\\ 
\end{aligned}
$$

To account for relativistic changes, divide by gamma : $$f=\frac{qB}{2\pi m} \sqrt{ 1- \frac{v^{2}}{c^{2}} }$$


Now there are other types too 


[[Betatron]] 
[[Scintillation detector]] 
[[Nuclear reactions]] 
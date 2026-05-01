<center> <font size=6>ISM Note 2</font></center>
<center><font size=4>Yang Chen</center>
<center><font size=4>3/7/2026</center>


# 1. Spiral galaxies (continued)

The Toomre's Q parameter is a very important parameter to analyze the stability of the disk, and it is defined by $Q = \frac{c_{s} \kappa}{\pi G \Sigma}$, where $c_{s}$ is the sound speed, $\kappa$ is the epicyclic frequency, which is defined by $\kappa = \sqrt{\frac{2 \Omega}{r} \frac{d \Omega}{d r}}, and $\Sigma$ is the surface density. If $Q < 1$, the disk is gravitationally unstable, and if $Q > 1$, the disk is gravitationally stable, while if $Q \approx 1$, the disk is marginally stable.

The unstable means the gas will fragment into clumps and then collapse to form stars. Since the gas mainly flow along the spiral arms, we can observe many stars in the arms of the spiral galaxy. 

Note that the Toomre's Q is not the only criterion to analyze the stability of the disk, for example, if $Q > 1$, the disk is either linearly stable or nonlinearly unstable. From the formulation of the Toomre's Q, we can see that thermal pressure + rotation can stabilize the disk, and sometimes the $v_{\text{turb}}$ can replace the sound speed $c_{s}$, which means the turbulence can also stabilize the disk, in other words, the turbulence can support the gas against collapse. To give an intuitive picture, the turbulence somehow describes the random motion of the gas, which is like what the thermal pressure does.


# 2. Elliptical galaxies

The elliptical galaxies are almost spherical, and NFW profile is a good description for the density distribution of the elliptical galaxies, which is given by $\rho(r) = \frac{\rho_{0}}{\frac{r}{r_{s}}(1+\frac{r}{r_{s}})^{2}}$, where $\rho_{0}$ and $r_{s}$ are two parameters, and here $r_{s}$ is the core radius, it is usually about 1-2 kpc. The NFW profile is a cuspy profile, which means the density increases sharply as $r$ decreases. 

The below figure shows the NFW profile
<figure style="text-align: center;">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8c/NFW_profile.png/300px-NFW_profile.png" alt="NFW profile">
    <figcaption>Fig 1. The NFW profile.</figcaption>
</figure>


The spherical shape of the elliptical galaxies means they are not supported by rotation, so the question here is: what supports the elliptical galaxies against collapse? The answer is the random motion or "heat". Quantitatively, $v_{\text{rot}} \leq 0.1 \sigma$, means the rotation velocity is much smaller than the random motion. 

Since the elliptical galaxies are spherical, we can not abstract them as a 2d obnject again but only as a 3d object. We can write down the hydrostatic balance equation for the elliptical galaxies, which is given by $\frac{d(\rho \sigma^2)}{dr} = -\frac{GM(r)\rho}{r^{2}}$, and if we replace $\sigma$ with $v_{\text{rot}}$, then we can get the turbulence equation. 


Why spirals and ellipticals are so different? The first clue is because of the early star formation vs late star formation. The spirals are the early-types, while the ellipticals are the late-types. There exis the transformation from spirals to ellipticals, the early star formation can release a large amount of energy, which can heat the gas and then get the random motion stronger, so the galaxy can be supported by the random motion more than rotation, and then the galaxy can transform from a spiral to an elliptical. The second clue is the environmental effects. For example, the galaxy can be affected by the mergers. The mergers can destroy the angular momentum and cause star burst, thus transform the galaxy from a spiral to an elliptical. 


# 3. Star-forming galaxies vs quiescent (passive) galaxies

We can also divides the galaxies into star-forming galaxies and quiescent (passive) galaxies. This classification is based on the star formation rate (SFR) of the galaxies $\dot M_*$. We have another quantiy named the specific star formation rate (sSFR) $ \text{sSFR} = \frac{\dot M_*}{M_*} $, and is a good indicator to distinguish the star-forming galaxies and quiescent galaxies. The star-forming galaxies have a high sSFR, which is typically about $\geq 10^{-11} \text{yr}^{-1}$. For our Milky Way, it is star-forming, and its sSFR is about $10^{-11} \text{yr}^{-1}$. 

The active galaxies we usually say it is blue, while the quiescent galaxies we usually say it is red. Interestingly, though the most spirals are star-forming, there are also some red spirals, which are quiescent. The reason for the red spirals might be that the gas in the red spirals is heated by the AGN feedback.

## active galaxy

The "active" here does not mean the star-forming, but small, highly energetic, non-stellar events within the galaxy. These events are usually in the radio band. One example of the active galaxy is the Seyfert galaxy, which is spiral having bright nuclei cannot be explained by stars. Another example is the radio galaxy, which has double radio lobes. Also there is quasars, namely quasi-stellar objects, which are very bright. All these active galaxies can be explained by AGN, namely active galactic nuclei. 




# 4. Stellar dynamics


We start from the distribution function $f(\mathbf{x},\mathbf{v},t) = \frac{dN}{d^3 x d^3 v}$, which describes the number of stars in the phase space. Then we want to study the evolution of the distribution function, and the equation governing the evolution of the distribution function is called the Vlasov equation, which is given by 
$$\frac{\partial f}{\partial t} + \frac{\partial \mathbf{x}}{\partial t} \cdot \frac{\partial f}{\partial \mathbf{x}} + \frac{\partial \mathbf{v}}{\partial t} \cdot \frac{\partial f}{\partial \mathbf{v}} = 0$$
where $\Phi$ is the gravitational potential. 
And 
$$\frac{\partial \mathbf{x}}{\partial t} + \mathbf{v} \cdot \nabla_{\mathbf{x}} f + \mathbf{g} \cdot \nabla_{\mathbf{v}} f = 0$$
where $\mathbf{g} = -\nabla \Phi$ is the gravitational acceleration.

Note that we are in a 6d phase space which is difficult to deal with, so we can integrate the distribution function over the velocity space first and get
$$\int \frac{\partial f}{\partial t} d^3 v + \int \mathbf{v} \cdot \nabla_{\mathbf{x}} f d^3 v + \int \mathbf{g} \cdot \nabla_{\mathbf{v}} f d^3 v = 0$$

The first term is $\frac{\partial}{\partial t} \int f d^3 v = \frac{\partial n}{\partial t}$, which is the time derivative of the number density. The second term is $\nabla_{\mathbf{x}} \cdot \int \mathbf{v} f d^3 v = \nabla_{\mathbf{x}} \cdot (n \langle \mathbf{v} \rangle)$, where $ \langle \mathbf{v} \rangle = \frac{\int \mathbf{v} f d^3 v}{\int f d^3 v}$ is the mean velocity. The third term is $\int \mathbf{g} \cdot \nabla_{\mathbf{v}} f d^3 v = 0$ because of the boundary condition that $f$ goes to zero as $v$ goes to infinity. 

(The course is up to 01:52:31, continue tomorrow)

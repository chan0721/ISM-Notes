<center> <font size=6>ISM Note 10</font></center>
<center><font size=4>Yang Chen</center>
<center><font size=4>4/30/2026</center>


# Eddington Luminosity

The gravitational radius is defined as

$$ r_g = \frac{GM}{c^2} $$

The Eddington luminosity can be given by   

$$ \frac{L_{Edd}}{4 \pi r^2} \frac{1}{c} \sigma_T = \frac{GMm_p}{r^2} $$

The RHS is the gravitational force, the first term on the LHS is the energy flux, combining with inverse of the speed of light gives the momentum flux. 

$\sigma_T$ is the Thomson scattering cross section, which gives the effective area of the photon captured by the proton. It is defined as

$$ \sigma_T = \frac{8\pi}{3} r_e^2 $$

where $r_e$ is the classical electron radius, defined as

$$ r_e = \frac{e^2}{4\pi \epsilon_0 m_e c^2} $$

We can derive the Thomson scattering cross section in the low-energy limit where the electron is scattered by photons, which gives 

$$ P \sim \frac{e^2 a^2}{c^3} $$

where $a = \frac{e E}{m_e} $ is the acceleration of the electron. The energy flux density is given by

$$ S = \frac{c}{4\pi} E^2 $$

With the energy equation $P = S \sigma_T$, we can derive the Thomson scattering cross section as given above.

Plugging this back the Eddington luminosity equation, we can derive the Eddington luminosity as

$$ L_{Edd} = \frac{4\pi GM m_p c}{\sigma_T} \sim 1.3 \times 10^{38} (\frac{M}{M_\odot}) \, \text{ergs}^{-1} $$


If we let $ L_{Edd} = \epsilon \frac{G M \dot{M}_{Edd}}{r}$, we can derive the Eddington mass flux as

$$ \dot{M}_{Edd} = \frac{4\pi}{\epsilon} \frac{r}{r_g} \frac{G M m_p}{\sigma_T c} $$

From the eddington luminosity equation, we can see that the balance is independent of the radius, which means that at all radii the balance will hold once $L \sim L_{Edd}$


## Sub-Eddington vs Super-Eddington Accretion


If the luminosity of the accretion flow is less than the Eddington luminosity, we call it sub-Eddington accretion. Similarly, if the luminosity of the accretion flow is greater than the Eddington luminosity, we call it super-Eddington accretion.


The Eddington luminosity gives the maximum accretion rate of a black hole. And the question is when will the sub-eddington and super-eddington accretion happen?

For the sub-eddington accretion, the answer is quite straightforward. If there is not enough gas supply, the accretion rate for the black hole will be low. For example, for the black hole in the edge of a galaxy, the gas supply is quite low, and the accretion rate is expected to be sub-eddington. 

For the super-eddington accretion, the answer is a little complicated. One reason for the super-eddington accretion is that the accretion is non-spherical and the gas is multiphase. Note that though Eddington luminosity is the theoretical limit for the luminosity of a black hole, super-eddington accretion is very common in our universe.


# Inflow of galaxy halo with cooling


Before we look at the inflow of the black hole, we look at the inflow at the galaxy halo scale first, which is $ \sim 10^2 $ kpc.

The big picture is, the gas will flow along the cosmic large scale structure and accrete onto the galaxy halo while losing its energy through cooling. So what will happen under this picture?


## Virial theorem

The virial theorem applies to a stable system where the particle are bounded by conservative forces. The virial theorem is given by

$$ 2 \langle T \rangle + \langle U \rangle = 0 $$

where $T$ is the total kinetic energy and $U$ is the total potential energy.

The gas in the galaxy halo is CGM and can apply the virial theorem. We solve the virial temperature of the gas in the galaxy halo as

$$ T_{vir} \sim \frac{\mu m_p}{2k_B} v_c^2 $$

where $v_c = \sqrt{\frac{GM_{halo}}{R_{vir}}}$ is the circular velocity of the gas in the galaxy halo, $M_{halo} = M_{DM} + M_{baryon}$ is the total mass of the galaxy halo.

$\mu$ is the mean molecular weight, which means the average mass of the particles in the gas. For a fully ionized hydrogen gas, $\mu = \frac{1}{2}$ because there are two particles (proton and electron) for each hydrogen atom. For a fully ionized gas with 75% hydrogen and 25% helium, $\mu \sim 0.6$.

If the gas is stable and the thermal pressure balances the gravitational force, then the virial temperature is the temperature of the gas in the galaxy halo. 


## dynamical timescale

One important timescale is the free-fall timescale, which is given by

$$ t_{ff} \sim \frac{R_{vir}}{v_c} $$

Another important timescale is the cooling timescale, which is given by

$$ t_{cool} \sim \frac{k_B T_{vir}}{n \Lambda(T_{vir})} $$

So we have two scenarios of how the gas accretes onto the galaxy halo. 

The first scenario is the hot-mode accretion, where the cooling timescale is much longer than the free-fall timescale. The gas will flow into the galaxy halo and when $v > c_s$ the shock will happen and can convert the kinetic energy into thermal energy. The gas will be heated to the virial temperature and form a hot atmosphere in the galaxy halo. Therefore, the whole process is called the "virialization".

The gas near galaxy cools down gradually and accretes to galaxy via thermal instability. Analytical works show that for the hot-mode accretion to happen, we requires $M_{halo} \geq 10^{11.5} M_\odot$.

The second scenario is the cold-mode accretion, where the cooling timescale is much shorter than the free-fall timescale. Here a stable shock front cannot form and the cool, filamentary gas feeds the galaxy directly. The "virialization" process does not happen and we can know the halo does not reach a quasi stable thermal state.


In early universe, there are many small halos and the cold-mode accretion is dominant. 


Note that when some non-thermal pressure exists, the virial theorem can be modified as

$$ 2 \langle T \rangle + \langle (U_{grav} - U_{eff}) \rangle = 0 $$

where $U_{eff}$ is the effective potential energy contributed by the non-thermal pressure like turbulence pressure and magnetic pressure. This implies that the kinetic energy will become smaller so the virial temperature will become smaller.


# Shocks


Shocks are discontinuities caused by motions $v > c_s$. The place where the discontinuity occurs is called the shock front. The gas already shocked is called downstream, while the gas that has not been shocked is called upstream. There are two frames, the lab frame the shock front frame. 


We consider the shock front frame, and denote the upstream quantities as $v_1$, $n_1$, $P_1$, $T_1$ and the downstream quantities as $v_2$, $n_2$, $P_2$, $T_2$. We have the basic relations 

$$ v_1 > c_{s,1} $$
$$ v_2 < v_1 $$
$$ n_2 > n_1 $$
$$ T_2 > T_1 $$

And now we are going to ask quantitatively how much the velocity, density and temperature change across the shock front. This question can be answered by the shock jump conditions. 

From the mass equation, we have

$$ \rho_1 v_1 = \rho_2 v_2 $$

From the momentum equation, we have

$$ P_1 + \rho_1 v_1^2 = P_2 + \rho_2 v_2^2 $$

And we assume the shock is adiabatic which means no thermal energy loss, we have the energy equation

$$ \frac{1}{2} v_1^3 + \frac{\gamma}{\gamma - 1} \frac{P_1}{v_1} = \frac{1}{2} v_2^3 + \frac{\gamma}{\gamma - 1} \frac{P_2}{v_2} $$

where $\gamma$ is the adiabatic index.

We combine these three equations and we can derive the final shock jump conditions as

$$ \frac{\rho_1}{\rho_2} = \frac{\gamma - 1}{\gamma + 1} + \frac{2}{(\gamma + 1) M_1^2} $$

$$ \frac{P_2}{P_1} = \frac{2\gamma M_1^2 - (\gamma - 1)}{\gamma + 1} $$

$$ \frac{v_2}{v_1} = \frac{\rho_1}{\rho_2} $$

where $M_1 = \frac{v_1}{c_{s,1}}$ is the Mach number of the upstream flow.


For a strong shock limit $M_1 \gg 1$, the shock jump conditions can be simplified as

$$ \frac{\rho_1}{\rho_2} = \frac{\gamma - 1}{\gamma + 1} $$

$$ \frac{P_2}{P_1} = \frac{2\gamma M_1^2}{\gamma + 1} $$

$$ \frac{v_2}{v_1} = \frac{\gamma - 1}{\gamma + 1} $$


For a monatomic gas, $\gamma = \frac{5}{3}$, we have $\frac{\rho_2}{\rho_1} = \frac{v_1}{v_2} = 4$, and $\frac{T_2}{T_1} = \frac{5 M_1^2}{16}$. This means the downstream gas is much hotter than the upstream gas, where the upstream kinetic energy is converted into the downstream thermal energy.

For the isothermal shock, the temperature does not change across the shock front, which means $T_2 = T_1$. The shock jump conditions can be simplified as

$$ \frac{\rho_1}{\rho_2} = \frac{v_2}{v_1} = \frac{P_1}{P_2} = M_1^{-2} $$


For the magnetic shock, the magnetic field line is parallel to the shock front, and due to flux freezing the magnetic lines will be compressed across the shock. This is called the quasi-perpendicular shock. 


For the oblique shock, the gas flow has a parallel motion to the shock front as well, and the velocity of the gas seems to be refracted across the shock front.


For the bow shock, the shock front is curved. The radius or the curvature of the shock front is given by 

$$ R_{shock} \propto \frac{P_{obstacle}}{P_{dynamic}} $$

where $P_{obstacle}$ is the pressure of the obstacle and $P_{dynamic} = \rho v^2$ is the dynamic pressure of the flow. 


Usually for the shock we have the contact discontinuity. For example, for the shock of the supernova explosion, we have the forward shock and the reverse shock. The forward shock is the shock front that propagates into the ISM, while the reverse shock is the shock front that propagates back into the supernova ejecta. The contact discontinuity is the boundary between the forward shock and the reverse shock, where the density and temperature can be discontinuous but the pressure and velocity are continuous.


The contact discontinuity(CD) is the interface between the ejecta and the ISM. That's the reason why we care about CD so much, because it is the place to distinguish SN ejecta and ISM. 

CD is unstable to fluid instabilities like Rayleigh-Taylor instability and leads to mixture. This consists the reason why the crab nebula can have the "finger like" structure.


# Riemann problem

We have the conservation equation for a quantity $u$ as 

$$ \frac{\partial u}{\partial t} + \nabla \cdot F(u) = 0 $$

And we have the initial condition as

$$ u(x, t=0) = \begin{cases} u_L & x < 0 \\ u_R & x \geq 0 \end{cases} $$

Then what is the solution for $u(x, t)$ at $t > 0$? This is the Riemann problem.

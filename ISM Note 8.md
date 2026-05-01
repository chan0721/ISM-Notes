<center> <font size=6>ISM Note 8</font></center>
<center><font size=4>Yang Chen</center>
<center><font size=4>4/16/2026</center>


# 1. Plasma Basics


First of all, we will consider the plasma wave. Consider a charge neutral media, where 

$$ n_+ = n_- = n $$

If we perturb the plasma, the electrons and ions will be separated, and then there will be an excess of charge density, which is given by 

$$ \rho = e n \xi $$ 

And the electric field can be derived by the Gauss's law, which is given by

$$ \vec{E} = 4 \pi e n \xi \hat{\vec{x}} $$


And from the Newton's second law, we can get the equation of motion for the electrons, which is given by

$$ m_e n \xi \frac{d^2 \xi}{dt^2} = (ne \xi) (4 \pi n e \xi) $$

This is a harmonics motion, the solution is given by $ \xi \propto e^{i \omega t} $, and here the frequency is called the electron plasma frequency, which is given by

$$ \omega_p^2 = \frac{4 \pi n e^2}{m_e} $$ 

Interestingly, this is also called the cut-off frequency in plasma. So what does thsi mean? It means that if you perturb the plasma with a frequency lower than the plasma frequency, the electron will rapidly bounce back and there will be no wave propagated in the plasma, only if you perturb the plasma with a frequency higher than the plasma frequency, the electrons are unable to respond to the perturbation, and then the wave can propagate. 


There is another important thing in plasma, which is the Debye shielding. Consider a test charge in the plasma, the test charge will attract opposite charges and repel like charges, and then there will be a cloud of opposite charges around the test charge, which can shield the electric field of the test charge. This means the charges are mobile and can shield out external charge field. So the question is, what is the length scale of the neutral region of the shielding? 
This is the Debye length, which is given by

$$ \lambda_D^2 = \frac{kT}{4 \pi n e^2} $$


For $ \lambda \gg \lambda_D $, the plasma can be treated as neutral. This is equivalent to saying that $ N_D = \frac{4 \pi}{3} n \lambda_D^3 \gg 1 $, which means there are many particles in the Debye sphere. 


The Debye length shows the competition between random motion and electromagnetic froce. If the temperature is high, the random motion is strong, and the Debye length is large, which means the shielding is not efficient. If the density is high, the electromagnetic force is strong, and the Debye length is small, which means the shielding is efficient. 


## Single particle motion

We consider the gyro motion, which is the motion of a charged particle in a magnetic field. The equation of motion is given by

$$  \frac{d \vec{p}}{dt} = q \frac{\vec{v}}{c} \times \vec{B} $$

If the particle is non-relativistic, $\vec{p} = m \vec{v}$, and the solution is given by

$$ v_{x,y} = v_\perp e^{i \Omega t} $$
$$ v_z = v_\parallel $$

where $\Omega$ is the gyro frequency, which is given by

$$ \Omega = \frac{q B}{m c} $$

The gyro radius or Larmor radius is given by

$$ r_g = \frac{\gamma v_\perp}{\Omega} $$


For a common astrophysical condition, the magnitude of some parameters are given by 

$$ B \sim \mu G $$
$$ E_{CR} \sim GeV $$
$$ r_g \sim AU $$


For example the solar wind, the gyro radius is about $ \sim 10^3 cm$, while for ISM it is about $\sim 10^3 cm$ which is much smaller than the scale we care about, and for IGM it is about $\sim 10^7 cm$. 


The gyro motion can be decomposed into two parts, the motion of guiding center plus the circular motion around the guiding center. 



## particle drifts


Let's impose an external electric field E on the plasma, then the equation of motion is given by

$$  \frac{d \vec{p}}{dt} = q (\vec{E} + \frac{\vec{v}}{c} \times \vec{B}) $$


Suppose the electric field is in the yz plane, and the magnetic field is in the z direction, then we can get the solution for the velocity, which is given by

$$ v_x = v_\perp e^{i \Omega t} - \frac{E_y}{B} $$
$$ v_y = i v_\perp e^{i \Omega t} $$
$$ v_z = v_\parallel + \frac{q E_z}{m} t $$

The first term is just the cyclotron motion, and the important thing is the second term, which is called the E cross B drift, which means if there exists an electric field, the particle drift will be perpendicular to both the electric field and the magnetic field. This is also called the side way drift, and it is given by 

$$ \vec{v}_E = c\frac{\vec{E} \times \vec{B}}{B^2} $$

This is independent of the charge and mass of the particle, so electrons and ions will drift together, so the plasma will still keep neutral and there's no net current density. 


## particle drifts with non-uniform magnetic field

The first is the gradient B drift. The magnetic moment is given by $\vec{\mu} = \frac{1}{2} \frac{m v_\perp^2}{B} $, and the force is given by $\vec{F} = - \nabla (\vec{\mu} \cdot \vec{B}) $, so the drift velocity is given by

$$ \vec{v}_{\nabla B} = \frac{ v_\perp^2}{2 \Omega} \frac{\vec{B} \times \nabla B}{B^2} $$ 

This is related to the perpendicular velocity of the particle.

Another drift is the curvature drift. The curvature is defined as 

$$\vec{\kappa} \sim \frac{\vec{R}}{R} $$

The curvature drift is given by

$$ \vec{v}_c = - \frac{v_\parallel^2}{\Omega R} \frac{\vec{B} \times \vec{\kappa}}{B} $$ 

which means that if the magnetic field lines are curved, the particle will drift due to its inertia, and this is related to the parallel velocity of the particle. Essentially, it is kind of a centrifugal force.


# 2. Adiabatic invariants


If the magnetic field is a constant or it changes slowly compared to the gyro motion, then there are some quantities that are conserved, which are called the adiabatic invariants. The first adiabatic invariant is the magnetic moment, which is given by

$$ \mu = \frac{1}{2} \frac{m v_\perp^2}{B} $$

So why does this quantity is conserved? We can understand it from the Maxwell's equation. So if the magnetic field changes slowly, which means

$$ \frac{1}{B} \frac{d B}{d t} \ll \Omega $$

Then we can get the electric field by the Faraday's law, which is given by

$$ \oint \vec{E} \cdot d \vec{l} = - \frac{1}{c} \int \frac{\partial \vec{B}}{\partial t} \cdot d \vec{S} = - \frac{1}{c} \frac{d B}{d t} \pi r_g^2 $$

The left hand side is the work done by the electric field, and with the Newton's second law, we can get the change of the kinetic energy, which is given by

$$ \frac{d}{dt} (\frac{1}{2} m v_\perp^2) = \frac{q \Omega}{2 \pi} \frac{\pi r_g^2}{c} \frac{d B}{d t} = \mu \frac{d B}{d t} $$


then the definition of the magnetic moment tells

$$ \frac{d \mu B}{d t} = \frac{d}{dt} (\frac{1}{2} m v_\perp^2) $$

Combining these two equations, we can get $ \frac{d \mu}{d t} = 0 $, this is the so-called first adiabatic invariant. 

Then we can have an important application of the first adiabatic invariant, which is the magnetic mirror. If the magnetic moment is a constant, then we can have

$$ v_\perp ^2 \propto B $$

And since the kinetic energy of the particle is also a constant, this means the parallel velocity of the particle in higher magnetic fields area will be smaller and smaller until zero, and since the Lorentz force still exist, this will reflect the particle back to the lower magnetic field region, this is the so-called particle trapping. 

We define a quantity $R_m = \frac{B_{max}}{B_{min}}$, which is called the mirror ratio, and the condition for the particle to be trapped is given by $ R_m > \frac{1}{\sin^2 \theta} $, where $\theta$ is the pitch angle of the particle, which is defined as $ \tan \theta = \frac{v_\perp}{v_\parallel} $. So if the particle has a large pitch angle, it is easier to be trapped. 



# 3. Magnetohydrodynamics (MHD)


If we want to describe the plasma on a large scale, we can use the magnetohydrodynamics (MHD) and need to add the Lorentz force term into the momentum equation, which is given by

$$ \rho \frac{d \vec{v}}{dt} = - \nabla P + \frac{1}{c} \vec{J} \times \vec{B} + \vec{F} $$

where $\vec{F}$ is the external force, and the magnetic force term can be rewritten as

$$ \frac{1}{c} \vec{J} \times \vec{B} = \frac{1}{4 \pi} (\nabla \times \vec{B}) \times \vec{B} = - \nabla (\frac{B^2}{8 \pi}) + \frac{1}{4 \pi} (\vec{B} \cdot \nabla) \vec{B} $$

The first term is the magnetic pressure, which means the magnetic energy carried by the magnetic field. And we can define a plasma beta, which is given by

$$ \beta = \frac{P_g}{P_B} $$

This is the ratio of the gas pressure to the magnetic pressure, and it tells us the relative importance of the gas pressure and the magnetic pressure. When we say a gas is "low beta", it means the magnetic field is dynamically important.

The second term is the magnetic tension, which is the force that tries to straighten the magnetic field lines. If we perturb the magnetic field lines, the magnetic tension will try to restore the magnetic field lines and this will create a wave, which is called the Alfvén wave. The Alfvén wave is a transverse wave, and the velocity of the Alfvén wave is given by

$$ v_A = \frac{B}{\sqrt{4 \pi \rho}} $$

This tells us how fast the information can propagate along the magnetic field lines. 


We need another equation to tell how the magnetic field evolves, which is given by the induction equation. First the Ohm's law is given by

$$ j = \sigma (\vec{E} + \frac{1}{c} \vec{v} \times \vec{B}) $$

where $\sigma \sim \frac{n e^2 \tau_{coll} u}{m}$ is the conductivity, and $\tau_{coll} \sim \frac{\lambda}{v}$ is the collision timescale. 

Then we plug the Ohm's law into the Faraday's law, and using the Ampere's law, we can get the induction equation, which is given by

$$ \frac{\partial \vec{B}}{\partial t} = \nabla \times (\vec{v} \times \vec{B}) + \eta \nabla^2 \vec{B} $$

where $\eta = \frac{c^2}{4 \pi \sigma}$ is the magnetic diffusivity or magnetic resistivity. 

We need to give a remark on the Ampere's law. We assume the displacement current term is negligible, one reason is the plasma is a good conductor, due to the Ohm's law, the electric field must be very small to avoid a large current, another reason is the plasma is non-relativistic, and the electric field is in the order of $v/c$ times the magnetic field, so it is negligible.


One important implication of the induction equation is the so-called flux freezing. The magnetic flux is given by

$$ \Phi_B = \int \vec{B} \cdot d \vec{S} $$

And the rate of change of the magnetic flux is given by

$$ \frac{d \Phi_B}{d t} = \int \frac{\partial \vec{B}}{\partial t} \cdot d \vec{S} + \int \vec{B} \cdot \frac{\partial}{\partial t} (d \vec{S}) $$

And since

$$ \frac{\partial }{\partial t} (d \vec{S}) = (\vec{v} \cdot \nabla) (d \vec{S}) - d \vec{S} (\vec{v} \cdot \nabla) $$

The first term is the stretching of the surface, and the second term is the expansion of the surface. Then we can plug it into the second term of the rate of change of the magnetic flux, and we can get

$$ \int \vec{B} \cdot \frac{\partial}{\partial t} (d \vec{S}) = \int \vec{B} \cdot \nabla \times (\vec{v} \time \vec{S}) = \int \nabla \times (\vec{B} \times \vec{v}) \cdot d \vec{S} = \oint (\vec{B} \times \vec{v}) \cdot d \vec{l} $$

Then we can plug the induction equation into the rate of change of the magnetic flux, and we can get

$$ \frac{d \Phi_B}{d t} = \int \eta \nabla^2 \vec{B} \cdot d \vec{S} $$

When $\eta \rightarrow 0$, the magnetic flux is conserved, which means the magnetic field lines through some loops are tied to plasma, not slipping off plasma. This is the so-called flux freezing. And when this condtion is satisfied, we say it is ideal MHD.


## resistive limit

The evolution equation of the magnetic field is the same as the standard diffusion equation, which is given by

$$ \frac{\partial \vec{B}}{\partial t} = \eta \nabla^2 \vec{B} $$

So if $\eta \neq 0$, the magnetic field can diffuse and slip off from the loop due to diffusivity, and the flux freezing will not hold. One direct result from this is the magnetic reconnection, which is the process that the magnetic field lines can break and reconnect, and this can convert the magnetic energy into thermal energy. This is important for the heating of the ISM. The magnetic reconnection can occur near the surface of the star and heat the gas.


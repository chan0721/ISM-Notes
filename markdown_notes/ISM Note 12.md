<center> <font size=6>ISM Note 12</font></center>
<center><font size=4>Yang Chen</center>
<center><font size=4>5/14/2026</center>


# Hydrodynamic instabilities


Start with a small perturbation and then it can grow exponentially. This is the phenomenon called hydrodynamic instability. There are two scenarios for this: One usually reaches saturation, and the other one can keep growing and runaway. For the first one, it implies the negative feedback while for the second one, it usually companies the positive feedback.


## Rayleigh-Taylor instability

The thing is, you have gravity downwards and heavy fluid on the top while light fluid on the bottom. If you give a perturbation to the interface, since the gradient of the pressure and the gradient of the density are not in line, there will develop a vorticity,

$$ \frac{d \vec{\omega}}{d t} \sim \frac{1}{\rho^2} \nabla \rho \times \nabla P $$

For the situation we described above, the fluid will enter first the linear growth phase, where the amplitude grows exponentially

$$ A \propto e^{\gamma t} $$

where $\gamma$ is the growth rate, which is given by

$$ \gamma \sim \sqrt{A k g} $$

where A is the Atwood number, which is defined as

$$ A = \frac{\rho_1 - \rho_2}{\rho_1 + \rho_2} $$

And k is the wavenumber which satisfies

$$ k \sim \frac{1}{L} $$


Then it will enter the nonlinear growth phase, and the secondary instabilities will develop and mix the interface. Finally, it will develop a turbulence.

To quantitatively describe the instability, we need to ask: what is the free energy driving the instability? It is not hard to see that this free energy is the gravitational potential energy, it converts to the kinetic energy of the fluid, which stands for the driven force. And after the turbulence develops, it can convert the kinetic energy to the thermal energy, which stands for the damping force. For this case, the driving force will finally balance the damping force, and the system will reach saturation. 


The first stage can be analytically described by the linear perturbation theory, which can derive the growth rate and the fastest growing mode. But for the second stage, we do not have an analytical theory, and most of the research work on this is guessing the dissipation term.


## Ritchmyer-Meshkov instability


The basic idea for this is very simple. The thing is, for the RT instability, the pressure gradient is provided by the gravity, but for the RM instability here, the pressure gradient is provided by the shock wave. 

So the common place for the RM instability is, in the ISM there are some dense clouds, and the supernova explosion will send a shock wave to the cloud and hit it, thus developing the RM instability.


## Kelvin-Helmholtz instability


So basically, you have a velocity shear and no gravity. If you give a perturbation to the boundary, the interface will roll up and develop into the turbulence. We can write down what is the growth rate, which is given by

$$ \gamma \sim k \frac{\sqrt{\rho_1 \rho_2}}{\rho_1 + \rho_2} |u_1 - u_2| $$

So one thing here is, the growth rate is proportional to the velocity difference, so no shear means no instability. And another fact is, suppose we have some tension on the interface, and usually the tension will suppress the instability, B-fields commonly play this role in astrophysical context.


## Magneric buoyancy


The magnetic field can also act as the seed for instability. The density scale height is given by

$$ H = \frac{k_B T}{\mu m_p g} $$

Suppose we have a pipe where the magnetic field is strong. Inside the pipe, we have $\rho_i$, $P_i$ and $B_i$, while outside the pipe, we have $\rho_e$, $P_e$ and $B_e = 0$. We assume the system is in pressure equilibrium, so we have

$$ P_i + \frac{B_i^2}{8 \pi} = P_e $$

And we also assume the system is isothermal, so we have

$$ T_i = T_e $$

Then obviously we have 

$$\rho_i < \rho_e$$

So according to the Achimedean principle, the buoyancy force is given by

$$ F_b = (\rho_e - \rho_i) g = \frac{B_i^2}{8 \pi H} $$

So what does this mean physically? It means the magnetic field is massless but can provide pressure. So the B-field will flow out of the pipe, but the tension in the fluid tries to bounce it back. So when

$$ g \delta \rho > \frac{B^2}{4 \pi R} $$

which means $R > 2H$, the flux tube is unstable to buoyancy. One example for this is the Solar flare.


## Parker instability

Assume you have parallel magnetic field lines, and the gravity is perpendicular to the field lines. And assume the ratio between the gas pressure and the magnetic pressure is a constant $\alpha$. So we can write down the pressure equation as

$$ (1+ \alpha_0) \frac{d P_{gas}}{d z} = - \frac{P_{gas}}{c_s^2} g $$

And then we can have

$$ \frac{P}{P_0} = \frac{\rho}{\rho_0} = \frac{B^2}{B_0^2} = e^{- \frac{z}{\Lambda}} $$

where $\Lambda$ is a new scale height, which is given by

$$ \Lambda = \frac{c_s^2 + v_A^2/2}{g} $$

So the magnetic field line will flow up due to buoyanct, and if we have the curvature 

$$ r \sim \frac{\lambda^2}{8 \delta z} $$

Then we can have

$$ \rho_i(\delta z) \sim \rho_0 e^{- \frac{\delta z}{H}} \sim \rho_0 (1 - \frac{\delta z}{H}) $$

$$ \rho_e(\delta z) \sim \rho_0 e^{- \frac{\delta z}{\Lambda}} \sim \rho_0 (1 - \frac{\delta z}{\Lambda}) $$

So the gas can slide down along the field lines and in the bottom you can see the gas accumulation. The condition for the instability is the buoyancy force is larger than the tension, which is given by

$$ \lambda^2 > \frac{16 \Lambda^2 \alpha}{(1 + \alpha)^2} $$



# Turbulence


## The Reynolds number

The Reynolds number is defined as

$$ Re = \frac{L u}{\nu} $$

The Reynolds number is the ratio between the inertial force and the viscous force. When $Re \geq 10^3$, the fluid is unstable to turbulence. This is the necessary condition for the turbulence.

One thing is, the Reynolds number is a relative number, which means it depends on the matetials and object we choose.


## Turbulence power spectrum

There are multiscale vortexes or eddies in the turbulence, and the large eddy will break into smaller eddies. The kinetic energy carried per unit volume is given by

$$ e_L \sim \rho u_L^2 $$

And the question is, what is the energy distribution function of the eddies? In other words, how much energy is carried by large eddies and how much energy is carried by small eddies? So to answer this question, we need to introduce a function

$$ E(k) \sim \frac{d e_L}{d k} $$

This function is called the energy spectrum, which describes how the kinetic energy is distributed in different scales. The power spectrum is firstly introduced by Kolmogorov. He assumes the turbulence is homogeneous, incompressible and stable.
Recall that the incompressible means the velocity is much smaller than the sound speed, so that the density perturbation is negligible so the density is nearly constant. 

Now consider a large eddy with a size of $L$, and define the energy transfer rate as

$$ \epsilon = \frac{e_L}{t_L} \sim \frac{\rho u_L^2}{L/u_L} \sim \frac{\rho u_L^3}{L} $$

Kolmogorov assumes the energy transfer rate is a constant, and this implies

$$ u_L \sim l^{1/3} $$

Then we can get the energy spectrum, which is given by

$$ E(k) \sim \frac{d e_L}{d k} \sim \frac{d (\rho u_L^2)}{d k} \sim k^{-5/3} $$




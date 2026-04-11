<center> <font size=6>ISM Note 6</font></center>
<center><font size=4>Yang Chen</center>
<center><font size=4>4/2/2026</center>



# 1. energy balance and temperature


Heating rate per HI is given by $\Gamma = \int_{\nu_1}^{\infty} \frac{4\pi J(\nu)}{h\nu} \sigma_{\text{ion}}(\nu) (h\nu - h\nu_1) d\nu \approx \phi \langle h(\nu - \nu_1) \rangle$, and heating rate per volume is given by $ H \approx n_{HI} \phi \langle h(\nu - \nu_1) \rangle$. And we assume ionization balance, so we have $n_{HI} \phi = n^2 x^2 \alpha(T)$. The recombination cooling rate is similarly given by $ \mathcal{L_{\text{rec}}} = n_{HI} \Sigma \int \sigma_{\text{rec}}(v)  v f(v) \frac{1}{2} m_e v^2 dv \approx n^2 x^2 \alpha(T) k_B T $. If the cooling must balance the heating, we then have $ H(T) = \mathcal{L_{\text{rec}}}(T) + \Sigma \mathcal{L_x}(T) $, and it is independent of the number density $n$. 



## multiphase ISM equilibrium


ISM cools via radiation, and this requires the ISM to be optically thin. We have to remark here that the equilibrium does not mean stable, they are different concepts. The net energy loss rate is given by $\mathcal{L_{\text{net}}} = n^2 \Lambda(T) - n^2 \Gamma(T)$, and from this we can derive the stability criterion, which is if $\frac{\partial \mathcal{L}}{\partial T} > 0$, then it is stable, otherwise it is unstable. This is easily understood, as long as you try to perturb the temperature and see how it would evolve. A sketch for the $\mathcal{L}(T)$ is shown as follows,

<figure style="text-align: center;">
    \includegraphics[width=0.5\textwidth]{multiphase.png}
    <figcaption>Fig 2. The multiphase ISM equilibrium.</figcaption>
</figure>


From this figure, we can see that the intermediate temperature range is stable, while others are unstable. But in the previous class we mentioned that the ICM gas has very high temperature, so it is thermally unstable, but we can still observe them. One reason is, the cooling time is very long, $t_{\text{cool}} \approx \frac{k_B T}{n \Lambda(T)}$, if the temperature is very high, and the density is very low, the cooling time can be very long, so the gas can still exist for a long time. Another reason is, there may exist some feedback mechanism, but this exact mechanism is still in research, this is the so called "cooling flow problem".


Note that we assume the ISM is in thermal equilibrium, but this is the global thermal equilibrium, which means the heating and cooling are balanced globally, but they may not be balanced locally. So the thermal instability can occur due to any thermal perturbations. 



# 2. Hydrodynamics


The main topic here is how can we describe the motion of a group of particles. The tool we use is the phas-space density / distribution function. The distribution function is defined as $f(\vec{x}, \vec{p}) = \frac{d N}{d^3x d^3p} $. First we can have the Boltzmann equation, which is given by $\frac{\partial f}{\partial t} + \vec{v} \cdot \nabla_x f + \vec{F} \cdot \nabla_p f = 0$, this equation means the change of the distribution function is due to the free streaming and the collision and it describes the conservation of particle numbers. The first thing we can do for the Boltzmann equation is to integrate over momentum space, and we can get $ \frac{\partial n}{\partial t} + \frac{\partial n \langle p \rangle}{m \partial x} = 0 $, where $n$ is the number density, and $\langle p \rangle$ is the average momentum. This is the continuity equation or mass equation. It can be easily seen that this continuity equation has two variables, so we need another equation to solve for these two variables. Then the second thing we can do is to multiply the Boltzmann equation by $\frac{p}{m}$ and then integrate over momentum space, and we can get $ \frac{\partial \langle p \rangle}{m \partial t} + \frac{\partial (v \times v + \langle w \times w \rangle)}{ \partial x} - n \vec{g} = 0$, where $w$ is the random velocity. Since we have $ P = \rho \frac{1}{3} Tr(\langle w \times w \rangle) = \rho \frac{1}{3} (w_x^2 + w_y^2 + w_z^2) = \rho w_x^2 = \rho w_y^2 = \rho w_z^2 $, here we assume the velocity distribution is isotropic. Then we can rewrite the stress tensor as $ \tilde{T} = \rho \langle \frac{p \times p}{m^2} \rangle = \rho (v \times v) + P \cdot I + \tilde{T}_{\text{vis}} $, where $\tilde{T}_{\text{vis}}$ is the viscous tensor. If $ \langle w_x w_y \rangle = \langle w_x \rangle \langle w_y \rangle = 0 $, it is statistically independent, then the $\tilde{T}_{\text{vis}} = 0$. And finally we can get the momentum equation, which is given by $ \frac{\partial }{\partial t} (\rho v) + \nabla \cdot \tilde{T} = \rho \vec{g} $. 


## Hydrostatic equilibrium

This means $\vec{v} = 0$, so we have $\nabla P = \rho \vec{g}$. For example, we consider the accretion disk around the black hole, the gravity is given by $\vec{g} = - \frac{GM}{r^2} \phi \hat{z}$, and we assume the radial component is balanced by centrifugal force, e.g. $g \approx \Omega^2 z$, then we can solve for the equation and get $\rho(z) = \rho_0 e^{- z^2 / 2 H^2}$, where the scale height is given by $H = \frac{c_s}{\Omega}$. The scale height is the characteristic height of the disk, and if the sound speed is high, which means the temperature is high, the scale height is large, and the disk is thick. If the sound speed is low, which means the temperature is low, the scale height is small, and the centrifugal force will dominate, and the disk is thin. 


Let's go back to the momentum equation, and we neglect the viscous term, then we have $ \frac{\partial }{\partial t} (\rho v) + \nabla \cdot (\rho v \times v + P \cdot I) = \rho \vec{g} $. We can do some math and plug in the continuity equation, and we can get $ \frac{\partial v}{\partial t} + (v \cdot \nabla) v = - \frac{1}{\rho} \nabla P + \vec{g} $. Then we can define a so-called Lagrangian derivative, which is given by $ \frac{D}{Dt} = \frac{\partial }{\partial t} + (v \cdot \nabla) $, then we can rewrite the above equation as $ \frac{D v}{Dt} = - \frac{1}{\rho} \nabla P + \vec{g} $. This is the Euler equation, which describes the motion of a fluid. 

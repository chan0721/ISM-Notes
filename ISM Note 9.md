<center> <font size=6>ISM Note 9</font></center>
<center><font size=4>Yang Chen</center>
<center><font size=4>4/26/2026</center>


# 1. Star formation (gravitational collapse)

We consider a gas cloud (protostar) with mass $M$ and radius $R$. When gravity dominates over thermal pressure, the cloud will collapse. 

$$ \frac{GMm}{R^2} > k_BT $$

where $m$ is the mean mass per particle. This gives us the Jeans mass:

$$ M_J \sim \left( \frac{k_BT}{Gm} \right)^{3/2} \rho^{-1/2} $$

where $\rho$ is the density of the cloud. This is the minimum mass required for a cloud to collapse under its own gravity. 

So the question is: for ISM the temperature and density are commonly constants or around some typical values, so the Jeans mass is also a constant. Then why do we have stars with different masses? The answer is the so-called fragmentation. When a cloud collapses, its density will increase, which will decrease the Jeans mass. This allows smaller fragments of the cloud to collapse and form stars with different masses. This fragmentation is the initial mass function (IMF) of stars. 

Another question is: at which point will the collapse stop? One important factor is the radiation pressure brought by the nuclear reactions. When collapse happens, the density will increase means the clouds become more optically thick and it will be harder for it to lose energy through radiation. This will lead to a higher temperature and thus increase the Jeans mass, which will stop the collapse.

We have several timescales of the collapse process. The free-fall timescale is the time it takes for a cloud to collapse under its own gravity, which is given by:

$$ t_{\text{ff}} \sim \sqrt{\frac{1}{G\rho}} $$


## cloud collapse (angular momentum)

Consider a galaxy with Keplerian rotation. 

$$ \Omega \sim \frac{1}{r^2} $$

This means the inner part will rotate faster than the outer part, which will transfer angular momentum from the inner part to the outer part. 


$$ \delta \Omega_{cloud} \sim \frac{d \Omega}{d R} \delta R \sim \frac{\Omega(R)}{R} r_{cloud} $$

If angular momentum is conserved, it will form a disk not a star, and the cloud will never collapse. So we need to transfer the angular momentum out of the cloud. This can be done through magnetic fields. 

Consider the flus freezing condition, the magnetic field lines will be dragged by the cloud, and we have

$$ B r^2 \sim \text{constant} $$

For the sun, this will give 

$$ B_{\odot} \ll B_{ISM} \left( \frac{R_{ISM}}{R_{\odot}} \right)^2 $$

The magnetic field of the sun is about $10^3$ Gauss, which is much smaller than the ISM magnetic field. The possible reason is the ambipolar diffuse. The B-field line will "slip" through the neutral component, so the magnetic field will decrease compared to the ideal case.


## vorticity equation

The vorticity equation is another way to write down the momentum equation in terms of the vorticity, which describes the evolution of the vorticity. This is given by

$$ \frac{\partial \vec{\omega}}{\partial t} = - (\vec{v} \cdot \nabla) \vec{\omega} + (\vec{\omega} \cdot \nabla) \vec{v} - \vec{\omega} (\nabla \cdot \vec{v}) + \frac{1}{\rho^2} \nabla \rho \times \nabla ( P + \frac{B^2}{8\pi} ) + \frac{1}{4\pi \rho^2} \nabla \rho \times (\vec{B} \cdot \nabla) \vec{B}\vec{B} $$

The first term is the advection term, which describes the transport of vorticity by the flow, if you do the volume integral of the whole space, this term will vanish. The second term is the stretching term, which describes the stretching of vorticity by the flow. The third term is the compression term, which has a negative sign before it. If we only have the first three terms, it is called barotropic flow. The fourth term is called baroclinic flow, which can generate vorticity, while the last term describes the magnetion tension to refrain the generation of vorticity.


## meaning of sound speed

We can define the so-called Mach number as 

$$ \mathcal{M} = \frac{v}{c_s} $$

We can describe several "information flow" cases with different Mach numbers with the following figure:
<figure style="text-align: center;">
    \includegraphics[width=0.5\textwidth]{Mach_number.png}
    <figcaption>Fig 1. Information flow with different Mach numbers.</figcaption>
</figure>

The supersonic case will create a shock, and when the shock happens, we can see some discontinuities. To see it better, let's look at the steady state of the force equation, which is given by

$$ \rho (\vec{v} \cdot \nabla) \vec{v} = - \nabla P  + \rho \vec{f} $$

If we some dimension analysis and make the gradient P term which acts as the inertia to have dimension 1, we can get the dimension of the first term is $\frac{v^2}{c_s^2}$ and the dimension of the last term is $\frac{U_f}{c_s^2}$. So if $\mathcal{M} \gg 1$, the first term will dominate, you drive the flow so fast that there is no time for the flow itself to relax, and the flow will have jumps and discontinuities. 


# 2. Stellar winds (no ISM interaction)

First of all, we have the mass conservation condition, which is given by

$$ \rho v r^2 = \text{constant} $$

We can do the logarithmic derivative of the above equation, and we can get

$$ \frac{1}{v} \frac{dv}{dr} + \frac{1}{\rho} \frac{d\rho}{dr} + \frac{2}{r} = 0 $$

Then we can write down the momentum equation, which is given by

$$ \rho v \frac{dv}{dr} + \frac{dP}{dr} = \rho \frac{GM}{r^2} $$

With $\frac{d P}{d r} = c_s^2 \frac{d \rho}{d r}$, we can plug in the result from the mass conservation condition, and we can get

$$ \left( v - \frac{c_s^2}{v} \right) \frac{dv}{dr} = \frac{2 c_s^2}{r} - \frac{GM}{r^2} $$

We don't have an analytic solution for the above equation, but we can do some analysis for some scenarios. 

First, when $v = c_s$, since the derivative of the velocity will not blow up, we can get the critical point, which is given by $r_s = \frac{GM}{2 c_s^2}$. This is the so-called sonic point, which is the point where the flow speed equals the sound speed. 

Second, when $r > r_s$, we assume the wind is isothermal, so we have $c_s^2 = \text{constant}$, and when $r \gg r_s$, we can get $v^2(r) \sim 4 c_s^2 \ln \frac{r}{r_s}$. So we can see from this that outside the sonic point the flow becomes supersonic but the Mach number will only be a few and not by too much. 

Third, when $r < r_s$, the gravity dominates, we can derive a solution with $ \frac{d v}{d r} > 0$ and $ v^2 < c_s^2$. And the asymptotic equation is given by

$$ \frac{v^2}{c_s} \frac{d v}{d r} = - \frac{GM}{r^2} $$

And it seems like gravity drives out the wind. 


Now we consider the stellar wind penetrates through the inhomogeneous ISM. When the stellar wind is blowed out from the star, it will interact with the cloud and have something called "wind-cloud interaction". This will create turbulence and may affect the evolution of the cloud. 


## inflow

Basically the inflow is triggered by gravity. The energy changing rate is given by

$$ \dot{E_g} \sim \frac{GM \dot{M}}{r} $$

where $\dot{M}$ is the mass accretion rate. And the luminosity of the accretion is given by

$$ L_{\text{acc}} \sim \epsilon \dot{E_g} \sim \epsilon \frac{GM \dot{M}}{r} $$

where $\epsilon$ is the radiation efficiency. From this we can compute the radiation temperature 

$$ \sigma T^4 \sim \frac{L_{\text{acc}}}{4\pi r^2} $$

The stellar mass BH has $T \sim 10^7$ K, and the supermassive BH has $T \sim 10^{4 - 5}$ K.  


## Bondi accretion (1D spherical)

The Bondi accretion is a smooth and adiabatic inflow. The mass accretion rate is given by

$$ \dot{M} = 4\pi r^2 \rho(r) v(r) $$

And with $P \propto \rho \gamma$ and $ c_s^2 = \frac{\gamma P}{\rho} $, we can get the following equation:

$$ \frac{1}{\rho} \frac{d P}{d r} = \frac{\gamma }{\gamma -1} \frac{d}{d r} (\frac{P}{\rho}) $$

Then we can plug in the above equation into the momentum equation, and we can get

$$ \frac{v^2}{2} + \frac{1}{\gamma - 1} c_s^2 - \frac{GM}{r} = \text{constant} $$

When $r \rightarrow \infty$, we have $v \rightarrow 0$ and $c_s \rightarrow c_{s, \infty}$, so we can get the constant is given by 

$$\frac{1}{\gamma - 1} c_{s, \infty}^2$$

And when $r \rightarrow r_s$, we have $v = c_s$, then we can get 

$$ \frac{1}{2} c_s^2(r_s) + \frac{1}{\gamma - 1} c_s^2(r_s) + 2 c_s^2(r_s) = \text{constant} $$ 

Combining the above two equations, we can get the relation between the sound speed at the sonic point and the sound speed at infinity, which is given by

$$ c_s^2(r_s) = \frac{2}{5 - 3\gamma} c_{s, \infty}^2 $$

And plug this into $P \propto \rho \gamma$ and $ c_s^2 = \frac{\gamma P}{\rho} $, we can get

$$ \rho(r_s) \sim \rho_{\infty} \left( \frac{c_s(r_s)}{c_{s, \infty}} \right)^{\frac{2}{\gamma - 1}} $$

Finally we can get the Bondi accretion rate, which is given by

$$ \dot{M} = 4\pi r_s^2 \rho(\infty) c_{s, \infty} \left( \frac{c_s(r_s)}{c_{s, \infty}} \right)^{\frac{\gamma + 1}{\gamma - 1}} $$

From this we can get

$$ \dot{M} \propto M^2 \rho_{\infty} c_{s, \infty}^{-3} $$

And the Bondi radius is given by

$$ r_B = \frac{GM}{c_{s, \infty}^2} $$

It shows the region where gas can be captured by gravity. For the supermassive BH, the Bondi radius is about $ 10 - 100 $ pc. When the gas is within the Bondi radius, it will be captured by the gravity of the BH and eventually accrete onto the BH forming an accretion disk. 


## Eddington luminosity

We have a definite gravitational radius (Bondi radius) $ r_g = \frac{GM}{c_{s, \infty}^2} $. The luminoisity is given by

$$ L = \epsilon \frac{GM \dot{M}}{r_g} \frac{r_g}{r} = \epsilon \frac{r_g}{r} \dot{M} c_{s, \infty}^2 $$

For the bright quasars, the luminosity can be as high as $10^{46}$ erg/s, and the mass accretion rate can be as high as $0.35 M_{\odot}/\text{yr}$. 

So the question is: what's the luminosity at which accretion flow stops?

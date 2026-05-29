<center> <font size=6>ISM Note 14</font></center>
<center><font size=4>Yang Chen</center>
<center><font size=4>5/28/2026</center>


# Cosmic rays(continued)

We know from the last class that the gyro radius is given by

$$ r_g \sim \frac{c p_\perp}{q B} \sim  $$

We can then define a quantity named rigidity, which is given by

$$ R = \frac{c p_\perp}{q} $$

So we can get

$$ r_g = \frac{R}{B} $$

(Q1: Why do we care about GeV cosmic rays? There are two reasons, need to check them)


## Origin of Cosmic Rays

This is related to the so-called particle acceleration. This can be usually divided into two stages. 

First stage, acceleration of low energy particles by large scale E field. It has two main sources, the first one is the magnetic reconnection, the other one is the unipolar dynamo.


## Magnetic Reconnection

A sketch for the magnetic reconnection is as follows

<figure><style="text-align: center;">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6e/Cosmic_ray_spectrum.svg/2560px-Cosmic_ray_spectrum.svg.png" width=500>
    <figcaption>Magnetic Reconnection</figcaption>
</figure>

The first equation we can write out is teh mass equation or continuity equation, which is given by

$$ v_{in} L \sim v_{out} l $$

And we assume the outward kinetic energy is the Alfven speed, which means

$$ v_{out}^2 \sim v_A^2 \sim \frac{B^2}{4 \pi \rho} $$

And combining the Ohm's law and the induction law, we can get

$$ \frac{B}{l} sim \frac{4 \pi}{c} \sigma E $$

Thus we can get the $ \vec{E} \times \vec{B} $ drift, 

$$ \vec{v}_{in} = c \frac{\vec{E} \times \vec{B}}{B^2} \sim c \frac{E}{B} \frac{e^2}{4 \pi \sigma l} \sim \frac{\eta}{l}  $$

$$ v_{in}^2 \sim \frac{v_A \eta}{L} $$

$$ l^2 \sim \frac{\eta L}{v_A} $$


The spontaneous reconnection rate can be calculated from the Sweet-Parker model. Lundquist number gives

$$ S = \frac{L v_A}{\eta} \geq 10^{10} $$

This number is too large that the magnetic reconnection can hardly happen. And in reality the rate is much larger than that expected from the Sweet-Parker model, and still remains a problem: Why is the rate much larger than that given by Sweet-Parker model?


### Possible Solutions

One is the plasmoid instability, which is also called the tearing instability. The magnetic lines can be streched and have some oscillations, the magnetic island will be generated in the magnetic lines, and this will cause the $L$ appeared in Sweet-Parker model to be much smaller.

Another possible one is the turbulence. The turbulence can twist the magnetic lines as well and work like the plasmoid instability. 


## Unipolar Dynamo

This usually happens to massive rotating compact objects, like the pulsar and accretion disks. We have

$$ \vec{E} \sim \frac{1}{c} \vec{v}_{rot}  \times \vec{B} $$


The second stage, we have two main processes. 

### Fermi II acceleration

The first one is the so-called Fermi II acceleration(stochastic). Recall that we have learned the magnetic mirror, where the magnetic moment is given by

$$ \mu = \frac{p_\perp }{2 \gamma m B} $$

and is conserved.

So imagine in a MHD turbulence, there are some regions where the magnetic field is large, and the particles will bounce back between the magnetic mirrors and get accelerated. This is the Fermi II acceleration. 

There are roughly two cases for the collision, one is the head-on collision, and the other one is the overtaking collision. Theses two cases seem to be symmetric so where does the acceleration come from? The answer is, there possbility are different, the head-on collision has a higher flux and thus have a larger rate, and this will finally lead to the acceleration.
The net energy change is given by

$$ \frac{d E}{d t} \sim \frac{v_0 + v_m}{L} 2m v_m (v+v_m) - \frac{v_0 - v_m}{L} 2m v_m (v-v_m) \sim \frac{E}{t_{coll}} \left ( \frac{v_m}{v} \right )^2 $$

This is the second order energy change, so it is called Fermi II acceleration. After $p$ times of collisions, we have

$$ E_p \sim E_0 \left ( 1 + \frac{v_m^2}{c^2} \right )^p $$

We assume the particle escape chance is $\eta$, and the escape timescale is $\tau$, then we have

$$ \eta \sim \frac{t_{coll}}{\tau} $$

So the number of particles at energy $E_p$ is given by

$$ E_p f(E_p) = N_0 P_0(p) - N_0 (1- \eta)^p $$

$$ \ln [E_p f(E_p)] = const + p \ln (1- \eta) \sim const - p \eta $$

And we can get

$$ f(E_p) \propto E^{-(1 + \frac{\eta c^2}{v_m^2})} $$

This is a power law but we know it is not a Maxwellian distribution so this is non-thermal. This process is not efficient.


### Fermi I acceleration

The second one is the so-called Fermi I acceleration(shock). This is also called the DSA(diffusive shock acceleration). The idea is, there is a MHD shock, and the particles can bounce back and forth between the upstream and downstream, and get accelerated. And since the upstream and downstream have different velocities, the particles can gain energy more efficiently than the Fermi II acceleration.

The energy change can be given by

$$ \ln \frac{E_p}{E_0} \sim p \frac{v_1 - v_2}{c}  $$

This is first order energy change, so it is called Fermi I acceleration. And we can get

$$ f(E_p) \propto E^s $$

where $s$ is given by

$$ s = \frac{v_1 + 2v_2}{v_1 - v_2} $$

For a strong shock, we have $v_1 / v_2 \sim 4$, and thus $s \sim 2$. 


## Cosimic Ray sources(GeV)


The first is the SNR, and its efficiency is about 10\% - 30\%, which means that 10\% - 30\% of the kinetic energy of the SNR can be converted into cosmic ray energy.

The second one is the AGN jets. Note that they can all generate shocks, so when you see a MHD shock, you can expect there is some cosmic ray generations.


## Cosmic Ray Transport

This is related to the so-called wave-particle interaction. The "wave" here means the Alfven wave.

The rough picture is, the cosmic rays are scattered by magnetic field irregularities, and are isotropized. The cosmic rays become isotropic due to the scattering by magnetic field, as we mentioned in last class.

The diffusion coefficient is given by

$$ \kappa_\parallel \sim \frac{v_{CR}^2}{\nu_s} $$

where $\nu_s$ is the scattering rate. A stronger scatter means a slower diffusion, and thus a stronger CR confinement. Therefore, we convert the CR transport problem into the source of magnetic field irregularities or the source of Alfven waves. 

The question is, what is the source of the Alfven waves? There are two main sources, the first is the self-confinement, which means the CRs themselves can excite the Alfven waves. It is called the cosmic ray streaming instability, also called the resonant instability, the resonant condition is given by

$$ \omega - k v_\parallel = +- \Omega $$

The growth rate is given by

$$ \gamma \sim \frac{\pi}{4} \Omega \frac{n_{CR}}{n_i} \left( \frac{v_D}{v_A} - 1 \right) $$

So if initially $v_D > v_A$, the instability can grow and the Alfven wave speed can grow until $v_D \sim v_A$. 


The second source is the extrinsic confinement, which is usually related to the turbulence. Confinement can reduce cosmic ray transport, but if there is a damping of the Alfven waves, then the cosmic ray will be less confined. There are several damping mechanisms, the first one is the ion-neutral damping, which usually happens in ISM. The second one is the non-linear Landau damping, which usually happens in ICM. The third one is the MHD turbulence cascade.


## Cosmic Ray Fluid Description

If we treat the cosmic rays as a fluid, then we can write down the cosmic ray equation as the fluid equation, which is given by

$$ \frac{\partial E_{CR}}{\partial t} + \nabla \cdot \vec{F}_{CR} = (\vec{v} + \vec{v}_{st}) \cdot \nabla P_{CR} + Q_{CR} + \Gamma_{CR} $$

where $E_{CR}$ is the cosmic ray energy density, $\vec{F}_{CR}$ is the cosmic ray flux,$\vec{v}_{st}$ is the streaming velocity, $P_{CR}$ is the cosmic ray pressure, $Q_{CR}$ is the cosmic ray source term, and $\Gamma_{CR}$ is the cosmic ray sink term.

The flux is given by

$$ \vec{F}_{CR} = (E_{CR} + P_{CR}) (\vec{v} + \vec{v}_{st}) - \kappa_\parallel \hat{\vec{n}} \hat{\vec{n}} \cdot \nabla P_{CR} $$

where $P_{CR} = \frac{1}{3} E_{CR}$ and $ \hat{\vec{n}} = \frac{\vec{v}}{|\vec{v}|} $. The flux is the streaming flux plus the diffusion flux. 

Thus the streaming velocity is given by

$$ \vec{v}_{st} = - \vec{v}_A \frac{\nabla P_{CR} \cdot \vec{B}}{|\nabla P_{CR} \cdot \vec{B}|} $$

Cosmic rays move along field lines and take the direction down the pressure gradient.


## Effect of Cosmic Rays

So what can cosmic rays do? First of all, they can provide pressure support, and the pressure gradient may accelerate the galactic outflows. 


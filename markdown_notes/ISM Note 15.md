<center> <font size=6>ISM Note 15</font></center>
<center><font size=4>Yang Chen</center>
<center><font size=4>6/4/2026</center>


# Effects of CR(continued)

Last time we mentioned that cosmic rays can provide non-thermal pressure support. Besides, the pressure gradient can drive galactic outflows to a very large radius. Simulation shows that, without cosimic rays, the outflow will go back to the galaxy, which is called galactic fountain. One core topic in modern astrophysics is to determine the range of feedback processes.

Cosmic rays can contribute to the bulk gas pressure, not random motion. In other words, the cosmic pressure can accelerate the gas without thermalizing it.


## Cosmic Ray Heating

The streaming heating rate is given by

$$ \Gamma_{stream} = \nabla P_{CR} \cdot \vec{v}_A $$

The Coulomb heating rate is given by

$$ \Gamma_{Coul} \sim 10^{-16} n_e n_{CR} $$

This is caused by Coulomb collisions between cosmic rays and thermal electrons. 

The hadronic heating rate is given by

$$ \Gamma_{had} \sim 10^{-16} n_p n_{CR} $$

This is also called p-p interaction, which is caused by the collisions between cosmic ray protons and thermal protons. This can produce gamms rays and can be observed by telescopes.


Note that CR cools much slower than gas, since it is always collisionless. This means the CR impact can be long-range and long-lasting. 


## Drive Turbulence and Amplify Magnetic Fields



The CR can cause the streaming instability can excite the Alfven waves, which can amplify the magnetic fields. 

There is another instability called Bell instability, e.g. in SNR, non-resonant instability, an extreme case of CR streaming instability. The non-resonant means $ r_L \cdot k > 1 $. 


## CR Ionization

For GeV cosmic rays, it can ionize deep GMCs, and even effect the formation of protoplanetary disks.



# Review

## Star formation

Gravitationally instable, which is the Jeans instability, the criterion is given by

$$ M > M_J \sim \left( \frac{k_BT}{Gm} \right)^{3/2} \rho^{-1/2} $$

But we know that if we only have collapse, the angular momentum and magnetic flux will be conserved, which can prevent the collapse. So we need mechanisms to get rid of the angular momentum and magnetic flux. 

For example, the molecular clouds are usually $ 10^2 M_{\odot} $ to $ 10^6 M_{\odot} $, $ T \sim 100 K$, $ n \sim 10^2 cm^{-3} $, and the free fall timescale is $ t_{ff} \sim 10 Myr$. From free fall and form stars, the SFR is about $ 500 M_{\odot} / yr $, but the observed SFR is only $ 1 M_{\odot} / yr $. So there must be some feedback processes to prevent star formation.


## Fragmentation

When a cloud collapses, its density will increase, which will decrease the Jeans mass. This allows smaller fragments to be unstable and collapse, this is the fragmentation process. The opacity is proportional to $\frac{M}{R^2}$ for fixed mass, the opacity will increase as the cloud collapses, which will make it harder for the cloud to lose energy through radiation. 


## Initial Mass Function(IMF)

The mass distribution of nearly born stars is called the initial mass function, the equation is given by

$$ \frac{dN(m,t)}{dt} = S(m,t) - \frac{N(m,t)}{\tau(m)} $$

where $S(m,t)$ is the star creation rate, and $\tau(m)$ is the lifetime of stars with mass $m$. Assume $S(m,t) $ does not change with time, we can get the solution as

$$ N(m,t) = S(m) (1 - e^{-t/\tau(m)}) $$

Obsevation gives the power law $S(m) \propto m^{-2.35}$ for $ m > 0.5 M_{\odot} $, for less massive stars, the trend becomes unclear. 


## The Intracluster Medium(ICM)

The ICM is high temperature, low density gas with $ T \sim 10^{7-8} K$. We can observe the ICM through X-ray emission, and the magnetic field is about $ 1 \mu G $. So the plasma beta is about $ \sim 100 $, which means the impact of magnetic field is not important.


## The Cooling Flow Problem

The cooling flow problem is that, 

$$ \dot{M}_{cool} \sim 10^3 M_{\odot} / yr \gg \text{observed} $$

One possible mechanism is the AGN feedback, and it might be the most important reason. Another possible mechanism is the turbulent heating. Other possible mechanisms include non-thermal pressure like cosmic rays.


## Multiphase ICM

From $H_\alpha$ emission, we can see $10^4$ K gas in filaments, which is much cooler than the usual ICM gas. 

One reason is the thermal instability. Though globally the heating and cooling are balanced, but locally these two can become unbalanced, which can lead to the thermal instability and the criterion is given by

$$ \frac{t_{cool}}{t_{ff}} < 10 $$

This means the free fall timescale is much longer so that the buoyancy oscillation will not create strong turbulence distorting the gas. The logic loop is, cooling will create cool gas, and the buoyancy oscillation will cause turbulence, which will distort the gas and thus prevent the cooling. 

When $$ t_{cool} \gg t_{ff} $$, the gas will ?


## The Circumgalactic Medium(CGM)

The CGM is also multiphase, its temperature is about $ 10^4 - 10^6 K $, which is cooler than the ICM. The reason is, the ICM is in a deeper gravitational potential well, and according to the virial theorem, the temperature will be larger than CGM.

The CGM is the host for feedback, including AGN feedback, SN feedback, stellar feedback and so on. 

The cool gas in CGM is unstable to hydrodynamic instabilities, but they are important fuels for star formation, so the cool gas survival is an important topic. 

Metals are important tracers. The cosmological inflow is pristine gas and usually has low metallicity, while the outflow/recycled gas is enriched by metals. The $\alpha$ elements include O, Ne, Mg, Si, C, Ca. This can track the ejecta of massive stars like type II SN and is recent enrichment. The iron element comes from type Ia SN. The delay time of type Ia SN is about $ 1 Gyr $, which is quite long, so this is late enrichment. Therefore, the type Ia SN can be usually observed in elliptical galaxies.





## Dust Grains

The dust grains has size of about $ \leq \mu m $, and the dust-to-gas mass ratio is about $ 0.01 $. The dust grains usually carries charges, and thus can be have the gyro motion. 

The dust has interactions with gas. Firstly, it can have the drag force and the Lorentz force. Secondly, the dust can have cooling, absorbing the UV and optical light and re-emitting in the infrared. This will cause the dust obscure and reddening of galaxies. Thirdly, the dust can be strongly coupled to radiation pressure. 


## Dust destruction

The dust can be destroyed by shocks, photons and thermal sputtering. For a cool/warm CGM, the sputting timescale is about $ t_{sp} \sim Myr$. So the question is, why dust can exist in the CGM? We know that the hot phase is dust-free, if all the cool gas comes from the hot phase, then there should be no dust in the CGM. So there must be some cool gas that comes from other sources, this question is similar to the multiphase CGM question.



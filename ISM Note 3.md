<center> <font size=6>ISM Note 3</font></center>
<center><font size=4>Yang Chen</center>
<center><font size=4>3/12/2026</center>


# 1. ISM observables (continued)

## Optical
For optical, we can observe the $10^3 - 10^4$ K gas. We can plot the collisional ionization equilibrium curve, which is as follows
<figure style="text-align: center;">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/3b/Collisional_ionization_equilibrium.png/300px-Collisional_ionization_equilibrium.png" alt="Collisional ionization equilibrium curve">
    <figcaption>Fig 1. The collisional ionization equilibrium curve.</figcaption>
</figure>

For ionization, there is also another ionization process called photoionization, which is caused by the photons. This process ont only depends on the temperature but also depends on the density. 

Usually in the dilute ISM, we have $t_{\text{ion}} < t_{\text{rec}} $, which means the gas is so dilute that it is hard for the electrons to find ions to recombine. For equilibrium, we assume $t_{\text{rec}} << t_{\text{dyn}} $, which means the recombination time scale is much smaller than the dynamical time scale. Physically, this means no matter how fast you drive the gas, the electrons can always find ions to recombine to reach the equilibrium. 


## Radio

For radio, we usually mean HI ( $T \leq 8,000 K$), the famous example is the 21 cm line. The 21 cm line is a ground state hyperfine structure transition. It is in the form of both emission and absorption. The abosorption process can be understand in a way shown in the below figure
<figure style="text-align: center;">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/4e/21cm_line.png/300px-21cm_line.png" alt="The 21 cm line">
    <figcaption>Fig 2. The 21 cm line.</figcaption>
</figure>

The spectrum shows many absorption lines because of the red shift. 

Another important radio emission process is the synchrotron emission, which is caused by the relativistic electrons spiraling around the magnetic field lines. If we drive the electron in a higher energy, then the emission will come over the radio band and into the X-ray band. 


## Infrared

For infrared, we can observe the $10-10^2$ K dust grains. They are solids embedded in the ISM.

## Millimeter

For millimeter, this is usually caused by the molecular gas $H_2$ rotational transition. The molecular gas is important for star formation.

## UV 

For UV, we can observe the $10^5 - 10^6$ K gas. 

## X-ray & Gamma-ray

For X-ray, we can observe the $\geq 10^6$ K ICM gas. So the question is, why can we see the X-ray easier in the ICM than in the ISM? The reason is that the largest gravity bounded structure in the universe is the galaxy cluster, and the gas around the galaxy cluster must be in very high temperature to against the gravity, so the gas in the galaxy cluster is usually hotter. 

There is another source for the X-ray band, which is SNR (supernova remnants). One more source for the X-ray band is the cosmic rays, which are highly relativistic particles. The cosmic rays can heat the ISM and then produce X-ray emission. 



# 2. Observe the ISM indirectly

## Plasma propagation (radio signals)

The first thing is the dispersion measure, which is defined by $DM \propto \int n_{e} dl$, which is an integral along the line of sight. Here $n_{e}$ is the electron number density. The dispersion measure can describe the change of the phase velocity of radio.  

Another measure is the rotation measure, which is defined by $RM \propto \int n_{e} B_{\parallel} dl$, where $B_{\parallel}$ is the magnetic field parallel to the line of sight. The rotation measure can describe the change of the polarization angle of radio. This is the so-called Faraday rotation. 

If we divide the rotation measure by the dispersion measure, we can get an estimate of the parallel magnetic field, which is given by $\langle B_{\parallel} \rangle = \frac{RM}{DM}$. If $\langle B_{\parallel} \rangle$ is small, this might not mean the magnetic field is small, but it might mean the magnetic field is quite tangled and random, so the positive and negative contributions can cancel each other.

One more measure is the emission measure, which is defined by $EM \propto \int n_{e}^{2} dl$. The emission measure can describe the change of the intensity of radio. 


# 3. Physical properties of the ISM


## The multiphase ISM

For neutral gas (atoms), e.g. HI, the temperature is about $10^3 - 10^4$ K. For molecular gas, e.g. $H_2$, the temperature is about $10-10^2$ K. For warm ionized gas, namely WIM, e.g. HII, the temperature is about $10^4-10^5$ K. For hot ionized gas, the temperature is about $\geq 10^6$ K. The multiphase gas should maintain the thermal pressure equilibrium, which means the numberdensity of different phases should be different, and simply satisfy $n_{1} T_{1} = n_{2} T_{2}$, where $n$ is the number density and $T$ is the temperature. 

The morphology of $H_2$ is clouds, filaments and sheets, since they have a higher density and a lower temperature. 


## Other components of the ISM

The ISM also contains the dust grains, and the ratio of the dust mass to the gas mass is about 1%. The dust grains can absorb or scatter stellar light, and radiate in the infrared, which is called dust obscured. This process is called radiative transfer. Besides, the dust can also contain heavy elements (metals), which can provide cooling for the ISM. 

The ISM also contains the cosmic rays, which are highly relativistic particles. The energy range (per particle) of the cosmic rays is about $10^9 - 10^{21}$ eV. We can divide the cosmic rays into many categories according to their energy. The first type is the low-energy cosmic rays, which are about $10^9 - 10^{11}$ eV ($1 - 100 Gev$), the second type is the high-energy cosmic rays, which are about $10^{11} - 10^{15}$ eV ($100 Gev - 1 PeV$), and the third type is the ultra-high-energy cosmic rays, which are about $\geq 10^{15}$ eV (1 PeV and above). We can draw the energy spectrum of the cosmic rays, which is as follows
<figure style="text-align: center;">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6e/Cosmic_ray_spectrum.png/300px-Cosmic_ray_spectrum.png" alt="The energy spectrum of the cosmic rays">
    <figcaption>Fig 3. The energy spectrum of the cosmic rays.</figcaption>
</figure>

From the figure, it is not hard for us to understand that in ISM we usually care about the Gev cosmic rays, which are in higher population. The cosmic ray energy density is about $1 eV/cm^3$. 


## Magnetic field in the ISM

The magnetic field in the ISM is about a few $\mu G$. The energy density of the magnetic field is also about $1 eV/cm^3$, which is comparable to the energy density of the cosmic rays and the thermal energy density of the ISM. This is called the equipartition of energy. In the ISM, the energy equipartition is between the kinetic energy, the thermal energy, and the non-thermal energy (cosmic rays and magnetic field). 


## Stuff related to stars

HII regions are the ionized gas around the young stars. We know the star formation happens in the molecular gas, but once the stars are formed, they can emit lights and ionize the gas around them, and then form the HII regions. The HII region is also called the Strömgren sphere, which is a sphere of ionized gas around the star. The radius can be calculated analytically, but we will leave it for the future course.

Another important thing is the planetary nebular, which is the gas ejected by the dying stars. One more important thing is the supernova remnants (SNR), which is the gas ejected by the supernova explosion. We can observe the SNR in different bands, such as radio, optical and X-ray, because the shock wave can heat the gas very efficiently. The SNR is also an important source for the cosmic rays, and one supernova can release about $10^{51}$ erg energy, and about 10% - 30% of the energy can be converted into the cosmic ray energy, other energy can be converted into the thermal energy and the kinetic energy of the ISM. 

One interesting thing is that though the cosimic rays energy fraction is only about 10% of the supernova energy, which is much smaller than the thermal energy fraction, but the cosmic rays can have a longer lifetime than the cooling time of the thermal energy, so that we can see the energy equipartition between the cosmic rays and the thermal energy. 

Molecular clouds are mainly composed of $H_2$, and they are the birthplace of stars. There are also some other molecules in the molecular clouds, such as CO, which is a good tracer for the molecular gas. The temperature of the molecular clouds is about $30-10^2$ K,and the typical mass is about $10^5 M_{\odot}$. Sometimes it can form a big molecular cloud, which is called the giant molecular cloud (GMC). The GMC is the collapse beds to star formation, and the typical mass of the GMC is about $10^5 - 10^6 M_{\odot}$. 

What is the efficiency of star formation? It is usually a few percent, which means only a few percent of the gas in the molecular clouds can be converted into stars. Why is the star formation efficiency so low? In other words, what can prevent the gas from collapsing? There are many factors that can play an important role, rotations, magnetic fields, turbulence. The magnetic fields forms a magnetostatic model, whose core idea is that the magnetic fields can provide support for the gas against collapse. 



# 4. ISM ecology

ISM is not static but highly dynamic and turbulent. The ISM can form stars and the stars can form stellar winds from the live stars and ejecta (supernova) from the dying stars. The feedback process from the ejecta is called metal enrichment, which can enrich the ISM with metals. 

## ISM in ellipticals

In the previous course, we know that the elliptical galaxies have low SFR. 
<center> <font size=6>ISM Note 13</font></center>
<center><font size=4>Yang Chen</center>
<center><font size=4>5/21/2026</center>

# Turbulence (continued)


## Kolmogorov power spectrum


We have derived the Kolmogrov power spectrum last lecture, which is given by 

$$ E(k) \propto k^{-5/3} $$

Since $k \sim \frac{1}{L}$, we can see that large eddies carry more energy than small eddies. 

The lower limit of the inertial range is called the injection scale, which corrsponds to the largest eddy. During the inertial range, the energy transfer is called the turbulence cascade. The upper limit of the inertial range is called the viscous scale, which corresponds to the smallest eddy. Below the viscous scale, the kinetic energy is converted into thermal energy.

We need to point out that the cascade occurs at 3 dimensions, while in 2 dimension the cascade is inversed, and we call it the inverse cascade.


## MHD turbulence

The most famous theory for the MHD turbulence is the so-called Goldreich-Sridhar 1995 theory. In this setup, they still assume the turbulence is incompressible, and the magnetic strength is strong.

We can decompose the velocity into two components, which are the parallel component and the perpendicular component. The critical balance condition is given by

$$ \frac{L_{\perp}}{\delta u} \sim \frac{L_{\parallel}}{v_A} $$

The LHS is the non-linear distortion timescale, and the RHS is the Alfven timescale. And since we know from the Kolmogorov power spectrum that 

$$ \delta u \propto L_{\perp}^{1/3} $$

We can get a power law

$$ L_{\parallel} \propto L_{\perp}^{2/3} $$

So what does this physically mean? The thing is, if you go to the small scale, e.g. $k_{\perp}$ is large, $k_{\parallel}$ does not grow as fast as $k_{\perp}$. Therefore, the parallel component is much smaller than the perpendicular component, which means the longer perturbation structure exist along B direction. So MHD turbulence is anisotropic and elongated along B field lines, especially at small scales.


We can understand it in another way. In the large scale, there is no time for the Alfven wave to propagate and different two points are disconnected, so you will not see strong MHD effect.


## The origin of astrophysical turbulence


The key thing here is, you have multiple scale of injection. For example, the cosmological inflow, virial shock, the merge of galaxy cluster are in Mpc scale and can cause turbulence; the galaxy related gravitational instability, galaxy merger, disk instability are in kpc scale and can cause turbulence, and the galactic feedback, e.g. supernova feedback, star formation feedback, AGN feedback can also cause turbulence; stellar winds, supernova remnants, and some ISM thermal instabilities can cause turbulence in pc scale; the fluid instabilities, plasma instabilities and cosmic rays can cause turbulence in sub-pc scale.  


## Consequence of turbulence


First of all, turbulence can create density fluctuations, this can then lead to thermal instability, gravitational instability etc. 

The second part is the so-called turbulent mixing. The turbulence can mix both the gas phase and the metal in a very efficient way.

Also, we know that the turbulence can provide pressure support, which is 

$$ P_{turb} \sim \rho v_{turb}^2 $$

And then, the turbulent heating is an important source of heating, which will convert the kinetic energy into thermal energy. 

And also, the turbulent dynamo can amplify the magnetic fields. 

The turbulence can also accounts for cosmic ray acceleration and transport. 


## Complexity beyond Kolmogorov


In astrophysical environment, the turbulence can be inhomogeneous in both space and time. The spatial inhomogeneity is called the intermittency.

And also, the turbulence can be anisotropic, like the MHD turbulence we have discussed, and also the turbulence in a gravitationally stratified medium. 

Besides, the turbulence can be compressible, non-adiabatic and so on. In all these cases, the Kolmogorov power spectrum will not hold.


## How to observe turbulence in ISM/CGM/ICM ...


The first thing is, we can measure them from absorption. Consider a light transmit through a medium, there will be some ions absorbing the light, and there will be a broadening of the absorption line. The broadening can be given by

$$ b_{obs} = \frac{2 k_B T}{m} + b_{nt} $$

where the first term is the thermal broadening, and the second term is the non-thermal broadening, which can be caused by the turbulence. 


The second thing of course is the emission. We ca measure the width of the emission line to observe the turbulence. However, in the diffuse gas we usually care about, the emission is very weak, unlike the absorption where we can use the bright background source.



# Cosmic Rays

The first question is, what are cosmic rays? Cosmic rays are highly relativistic particles, which can be protons, electrons, positrons etc. 

The distribution function of cosmic rays is nearly a piecewise power law, which is shown in the figure below.

<figure><style="text-align: center;">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6e/Cosmic_ray_spectrum.svg/2560px-Cosmic_ray_spectrum.svg.png" width=500>
    <figcaption>Cosmic ray spectrum. Credit: Wikimedia Commons.</figcaption>
</figure>

This distribution function is non-Maxwellian and non-thermal. The two part power law has different acceleration mechanism.

For galaxy evolution, we care about cosmis rays in GeV and mostly protons, that is because GeV cosmic rays have largest flux, and protons have much longer lifetime than electrons.


The cosmic rays are quite collisionless.Because the mean free path of cosmic rays is very large, which is usually $\lambda_{mfp} \sim 10^30 cm$ for GeV cosmic rays.

The cosmic rays are extremely low level of anisotropy, which is about $10^{-4}$, so the bulk motion is about $v_{bulk} \sim 10^{-4} c \ll c $. 

The escape time from galaxy can be estimated as 

$$ t_{esc} \sim \frac{H}{v_{bulk}} \sim 5 Myr $$

Therefore, the cosmic rays can remain in the galaxy for a long time and the feedback can be important.


## Gyro motion

The gyro radius of cosmic rays is given by

$$ r_g \sim \frac{p_\perp c}{q B} \sim \frac{2.2}{Z} \left(\frac{p_\perp}{10 GeV/c} \right) \left(\frac{B}{1 \mu G} \right) AU $$

The gyro radius is much smaller than the relevant galactic length, so the cosmic rays can stay in the galaxy for a long time.


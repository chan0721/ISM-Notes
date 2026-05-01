<center> <font size=6>ISM Note 1</font></center>
<center><font size=4>Yang Chen</center>
<center><font size=4>3/5/2026</center>

# 1. The interstellar medium (ISM)

The true name of this name should be the physics of the diffuse baryons, which is more precise to describe the content of this course. The "baryons" here refer to the normal matter in our universe, which is made up of protons, neutrons, and electrons. And over 99.99% of the baryons in the universe are in the form of plasma. The "diffuse" here means that the density of these baryons is very low, where the non-diffuse baryons are those in stars and other compact objects. The mean density of the ISM is about 1 particle per cubic centimeter (1 cm$^{-3}$). There are active interactions between the ISM and stars, the ISM can concentrate to form stars, and the stars can also inject energy and mass into the ISM through stellar winds and supernova explosions. What is the ratio of the total mass of the diffuse baryons to the total mass of the stars? Roughly it is about 1:1, that's the raw picture for the ISM.


## The big picture of our universe 

Initially the universe is mainly made of dark matter uniformly distributed. And then the quantum fluctuations acted as perturbations to the dark matter, which will cause the dark matter to shrink and grow by virtue of a positive feedback, which is the so-called gravitational instabilities. Then it will form the large scale structure of the universe, which is also called the cosmic web, and its characteristic scale is about $10^{2}$ Mpc. The cosmic web is like the skeleton of the universe, and the gas will flow through the filaments and fall into the dark matter halos motivated by the gravity. For astrophysicists, though we cannot observe the dark matter directly, we can observe the number densities of galaxies and stars to infer the distribution of dark matter. The gas flow along the filaments are called intergalactic medium (IGM).

The cosmic web image is as follows
![Cosmic web](D:/11639/ism_notes/cosmic_web.png)

In the DM halos, there are thousands of galaxies in the galaxy clusters, and the gas within the galaxy clusters is called the intracluster medium (ICM), and its characteristic scale is about $10^{1}$ Mpc. By the way, the galaxy clusters are the largest gravitational bounded structures in the universe. 

Then we have the galaxies, and the gas around the galaxies is called the circumgalactic medium (CGM), and its characteristic scale is about $10^{2}$ kpc. 

Finally, we have the ISM, which is the gas within the galaxies, and its characteristic scale is about $10^{1}$ kpc. This course will cover all the gases we mentioned above, which are all the diffuse baryons in the universe.


# 2. The galaxies

The galaxies can be classified into two categories, the spiral galaxies and the elliptical galaxies. They are also called normal galaxies. The first question is, what is the number density of the galaxies? The answer is given by the Schechter function, which is also known as the luminosity function of the galaxies. The Schechter function is given by
$$\Phi(L) = \frac{dn}{dL} = \Phi_{0} \left( \frac{L}{L_{*}} \right)^{-\alpha} e^{-L/L_{*}}$$

where $\phi_{*}$ is the number density of galaxies with milky way luminosity, $L_{*}$ is the milky way luminosity, and $\alpha$ is the faint-end slope. The Schechter function describes the number density of galaxies as a function of their luminosity. The characteristic luminosity $L_{*}$ is the luminosity at which the number density of galaxies starts to decline exponentially. The faint-end slope $\alpha$ describes how the number density of galaxies changes at low luminosities.

The sketch of the Schechter function is as follows
![Schechter function](D:/11639/ism_notes/Schechter_function.png)

From the image, we can see that the luminosity(x-axis) covered mainly 4 orders of magnitude, and for the region $$L/L_{*} > 10^{0} $$, there are normal galaxies, and since the elliptical galaxies are more massive while the spiral galaxies are less massive, the elliptical galaxies mainly occupy the right area of this regiion. And for the region $$L/L_{*} < 10^{0} $$, there are dwarf galaxies. The dwarfs are usully irregular shaped, because their mass are too small to power for the least free energy state. 

We can get a prediction of the luminosity function from the DM survey, but except for the turning point, the prediction overestimates the number density of galaxies, the reason for the "lower" real curve is mainly due to the feedback mechanism. But we will leave it to the future lectures to go into the details.


## Spiral / Disk galaxies

The spiral galaxies are very flat and we can abstract it as 2D disks. The face-on view and edge-on view sketches are as follows
![Spiral galaxies](D:/11639/ism_notes/spiral_galaxies.png)

We usually use surface density to describe the properties of the spiral galaxies, and the surface density is defined as $\Sigma = \int \rho(r,\phi,z) dz$, where $\rho$ is the volume density and $z$ is the vertical direction. Usually for a spiral galaxy, the surface density satisfies $\Sigma(r) \propto e^{-r/H}$, where $H$ is the scale length.

So why does it form a disk-like structure? The reason is about rotation. Horizontally, it is supported by rotation. Vertically, the galaxy does not shrink into a line because of random motion or thermal pressure to balance with the gravity. 

The rotational velocity roughly satisfies $v_{\text{rot}}(r) \propto \frac{GM(r)}{r}$, and then we can plot the rotational curve, which is as follows
![Rotational curve](D:/11639/ism_notes/rotational_curve.png)

The observational data is quite different from the theoretical prediction in the large r region, and the reason is that there is a large amount of dark matter in the outer region of the galaxy, which can provide extra gravity to support the rotation. Then we can define a quantity named baryon fraction $f_{b} = \frac{M_{\text{b}}}{M_{\text{total}}}$, and the common value of the baryon fraction for dwarfs is about 1%-5%, while for normal galaxies is about 5%-10%. 

### Spiral arms

Why do spiral galaxies have spiral arms? This is a kind of non-axisymmetric structure, but we can use Fourier decomposition to analyze it. The Fourier decomposition is given by
$$f(r,z,\phi) = \sum_{m=-\infty}^{\infty} f(r,z) e^{im\phi}$$
m is called the azimuthal number, and different m corresponds to different arm numbers. 

The reason for the formation of the spiral arms is various, and one is the density wave theory, one is the gravitational instability. The density wave theory is that the spiral arms are like traffic jams, which are not material arms, but the density waves. The gravitational instability is that the spiral arms are formed by the gravitational instability of the disk, which can be analyzed by the Toomre's Q parameter, which is given by
$$Q = \frac{c_{s} \kappa}{\pi G \Sigma}$$
where $c_{s}$ is the sound speed, $\kappa$ is the epicyclic frequency, which is defined by $\kappa = \sqrt{\frac{2 \Omega}{r} \frac{d \Omega}{d r}}, and $\Sigma$ is the surface density. If $Q < 1$, the disk is gravitationally unstable, and if $Q > 1$, the disk is gravitationally stable, while if $Q \approx 1$, the disk is marginally stable. 


#### $c_s$ sound speed

The sound speed tells you the transmission speed of the perturbation in pressure, while it is also a speed of information in the fluid. 
We can easily derive $P \propto \rho \gamma$, which means the thermal pressure is highly related to the sound speed.

#### $\kappa$ epicyclic frequency
The epicyclic frequency is the frequency of the small oscillation of a particle around its circular orbit. It corresponds to the rotation physically. 

From the Toomre's Q parameter and our disscussion above, we can see that thermal pressure + rotation can stabilize the disk, while the self-gravity($G\Sigma$) can destabilize the disk.

If the disk is gravitationally unstable, it will fragment into clumps, and the clumps will collapse to enhance the star formation.

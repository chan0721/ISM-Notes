<center> <font size=6>ISM Note 7</font></center>
<center><font size=4>Yang Chen</center>
<center><font size=4>4/9/2026</center>


# 1. Hydrodynamics (continued)

Last class we end with the lagrangian derivative, which is given by $ \frac{D}{Dt} = \frac{\partial }{\partial t} + (v \cdot \nabla) $, the partial derivative is the change of the quantity at a fixed point, which is an Eulerian description, while the lagrangian derivative is a total derivative, which is the change of the quantity following the fluid element. With that we can introduce the so-called Archimedes' principle, which tells us that the heavier fluid will sink, and the lighter fluid will float. This can be easily understood from the momentum equation.


We will now introduce the energy equation. Recall that the mass equation is the 0th moment of the Boltzmann equation, and the momentum equation is the 1st moment of the Boltzmann equation, then straightforwardly, we can get the 2nd moment of the Boltzmann equation, which is the so-called energy equation. But we will not write down it directly, instead we will try to write it in the conservation form, which is given by $ \frac{\partial E}{\partial t} + \nabla \cdot ((\frac{1}{2} \rhov^2 + \frac{5}{2} P) \vec{v}) = source $, notice that here the flux term contains another pressure term. Why for the extra pressure term? We can decompose it as $ \nabla \cdot (P \vec{v}) = P( \nabla \cdot \vec{v} )+ \vec{v} \cdot \nabla P $, the first term is the PdV work, and the second term is the work done due to the flow of the fluid. The source term usually did not disappear, even for the mass equation. For example, if the gas is around a black hole, the gas can be swallowed by the black hole and act as a sink term for the mass equation. For the energy equation, the source term not only contains everything in the momentum equation, but also contains the heating and cooling terms. 


There is another equation we can write down, which is the so-called entropy equation, physically this is the total energy equation substracts the momentum equation, so it describes the change of the internal energy. The entropy equation is given by $ \frac{3}{2} \frac{d \ln P}{dt} - \frac{5}{2} \frac{d \ln \rho }{dt} = 0 $, if we define the entropy as $ S = c_v \ln (\frac{P}{\rho^{5/3}}) $, then the above equation can be rewritten as $ \frac{dS}{dt} = 0 $, which means the entropy is conserved. The interesting point is, the gas can have adiabatic cooling or heating, but if we look at the entropy equation, we can see that these will disappear, so the change of the entropy is only due to the non-adiabatic cooling or heating. 


## Convection

Consider a blob in a stratified atmosphere, if we perturb the blob and let it move up, we need to tell whether the blob will fall back or continue to move up. Straightforwardly, these requires us to compare the density drop of the perturbed blob and the surrounding medium. Inside the blob, we know the entropy is conserved, and we assume the blob is in pressure equilibrium with the surrounding medium, so we have $ P_{\text{in}} = P_{z+\delta z} $, and $ S_{\text{in}} = S_{\text{z}} $. Outside the blob, we have $ P_{\text{out}} = P_{z+\delta z} $, and $ S_{\text{out}} = S_{z+\delta z} $. So by some simple derivation, we can get $ \frac{\partial S}{\partial z} > 0 $ is the stability criterion for the convection. If stable the blob will oscillate, and this frequency is the so-called Brunt-Vaisala frequency, which is given by $ N^2 = \frac{g}{c_p} \frac{\partial S}{\partial z} $. For example, the internal gravity waves in the atmosphere of the Earth is due to the convection, also names as G-modes. 


## Sound waves

We use the linear perturbation theory to analyze the sound waves. We assume the background is static, and we have $ \rho = \rho_0 + \delta \rho $, $ P = P_0 + \delta P $, and $ v = 0 + \delta v $. We plug these into the mass equation and get, $ \frac{\partial \delta \rho}{\partial t} + \rho (\nabla \cdot \delta \vec{v}) = 0 $, then we can do the Fourier transformation and assume $ \delta \approx e^{i(\vec{k} \cdot \vec{x} - \omega t)} $, and then we can get $ - i \omega \delta \rho + i \rho_0 \vec{k} \cdot \delta \vec{v} = 0 $. This tells us that the longitudinal component of the velocity is related to the density perturbation, and this component is equivalent to the compressive mode. If $ \vec{k} \cdot \delta \vec{v} = 0 $, the wave is only solenoidal, and there will be no density fluctuations. 


For the momentum equation, with the similar procedure, we can get $ - i \omega \rho_0 \delta \vec{v} + i \vec{k} \delta P = 0 $. We dotting $ \vec{k}$ on both sides, we can get $ - i \omega \rho_0 \vec{k} \cdot \delta \vec{v} + i k^2 \delta P = 0 $. Then we can plug in the result from the entropy equation, and finally we can get the dispersion relation for the sound wave, which is given by $ \omega^2 = c_s^2 k^2 $, where $c_s$ is the sound speed, which is given by $ c_s^2 = \frac{\gamma P_0}{\rho_0} $. So for a sound wave we know its group velocity is the same as its phase velocity, and it is a longitudinal wave.



## Convection (WKB)


We write again the momentum equation with a gravity source term, $ - i \omega \rho_0 \delta \vec{v} + i \vec{k} \delta P = \delta \rho \vec{g} $, and cross this equation with $\vec{k}$ twice, and assume $ \delta P = 0 $ and move the blob very slow, in that case, we can get $ i \omega c_p \frac{\delta \rho}{\rho} + \delta v_z \frac{d S}{d z} = 0 $, this tells us that the density response to vertical motion. Then we can derive the dispersion relation for the convection, which is given by $ \omega^2 = N^2 (1 - \bar{k_z}^2) $, where $N$ is the Brunt-Vaisala frequency, and $\bar{k_z} = \frac{k_z}{k}$. So if $k_z = 0$, $k_h \neq 0$, we can get $\delta v \neq 0$, and if $k_z \neq 0$, $k_h = 0$, we can get $\delta v = 0$, which means it cannot propagate vertically. So this is a transverse wave, and the wave package energy travels along the surface of constant phase. This is the internal gravity wave. 


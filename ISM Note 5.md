<center> <font size=6>ISM Note 5</font></center>
<center><font size=4>Yang Chen</center>
<center><font size=4>3/26/2026</center>


# 1. Radiative process (continued)

## Bremsstrahlung radiation (free-free radiation)

The Bremsstrahlung radiation is the radiation emitted by the free electrons when they are accelerated by the Coulomb field of the ions. The power emitted by a single electron is given by $P = \frac{2 e^2 a^2}{3 c^3}$, where $a$ is the acceleration of the electron. The emission of a large group of free electrons following the Maxwell-Boltzmann distribution. And the power spectrum plot is as follows: at high frequencies, the power is proportional to $e^{-h\nu/kT}$, which is called the high frequency cutoff, and this only corresponds to optically thin plasma. At low frequencies, tje gas is optically thick, and it is black body like, so the low energy limit is just the Rayleigh-Jeans limit, which is given by $ I_{\nu} \propto \nu^2$. Re-absorption here is important. For the mid-frequency range, $I_{\nu} \approx const$, and $\epsilon_{\nu} \approx Z^2 n_e n_i T^{1/2} $, where $Z$ is the charge number, $\epsilon_{\nu}$ is the volume emissivity. 

If you look at temperature higher than $10^6 - 10^7 K$, the radiation is dominated by the Bremsstrahlung radiation, and you can see the X-ray emission from the hot gas. 




# 2. Thermal states of the ISM

First of all, it is cooling. And here we only consider the optically thin gas. The cooling describes the net energy loss per unit time per unit volume, which is given by $\mathcal{L} = n^2 \Lambda(T)$, where $\Lambda(T)$ is the cooling function, or usually refered as cooling curve, which is in unit of $erg cm^3 s^{-1}$. The $n^2$ here means the cooling is a two-body process here. 

We can define a cooling timescale by $t_{\text{cool}} = \frac{E_{\text{th}}}{\mathcal{L}} = \frac{kT}{n \Lambda(T)}$. One cooling curve is given as follows
<figure style="text-align: center;">
    \includegraphics[width=0.5\textwidth]{cooling_curve.png}
    <figcaption>Fig 1. The cooling curve.</figcaption>
</figure>

From the above figure, we can give some discussion on the cooling curve. For $T \geq 10^7 K$, all elements are fully ionized, so the cooling is dominated by the Bremsstrahlung radiation, which is given by $\Lambda(T) \propto T^{1/2}$. For $ T \approx 10^4 - 10^7 K $, there is excitation of electron and then spontaneous de-excitation and emit photon, which is called the forbidden line. The forbidden line will only occur in the dilute ISM, the reason is, the excited electrons can survive for a long time, and then they can spontaneously de-excite and emit photon, while in the dense ISM, the excited electrons will be collisionally de-excited before they can spontaneously de-excite, in this case cooling is not efficient. The excitation is mainly of metals, so it is also called the metal line cooling. If the gas is metal rich, the cooling is much more efficient than the cooling poor. For $T \approx 10^4 K $, the cooling is mainly the hydrogen excitation. If we go to $T < 10^4 K$, the excitation of fine structure dominates the cooling, and it is in the band of infrared. If we go to $T > 10^9 K $, the cooling is dominated by the pair production, but nearly no gas can reach such a high temperature, unless the gas is in a special environment, so this is usually not important for the ISM.



Secondly, it is heating. The dominant energy in ISM involves the thermal energy, the turbulent enrgy, the cosmic ray energy, the magnetic energy, and the photon energy.

First, the turbulent heating/dissipation. $E_{\text{turb}} \approx E_{\text{th}}$. Second, the cosmic ray heating. WE will not discuss it in detail today and leave them to the future chapter. Third, the magnetic reconnection. The magnetic reconnection can convert the magnetic energy into thermal energy, and it is important for the heating of the ISM. The magnetic reconnection can occur near the surface of the star and heat the gas. Finally, the photoionization heating and photoelectric heating. Usually we can find these photoionization heating aroung young stars and AGN. The photoelectric heating is the process that the UV photon can hit the dust grain and get absorbed.


Heatin is much more complicated and much more difficult to handle than cooling. First of all, the heating dependence on parameters is much more complicated, since there are many different heating sources. Second, the heating and cooling are not balanced in general. 


## HII regions (spherical chicken)

The HII regions are the ionized regions around the young (O/B) stars. We can somehow derive the radius of the HII region analytically. The average over $\Omega$ is $J(\nu,r) \approx \frac{L_\nu}{4\pi r^2} e^{- \tau(\nu,r)}$. With that, let's conside what photons can ionize the ISM. As we all know, photons have energy higher than 13.6 eV can ionize the hydrogen. Then the cross section is $\sigma_{\text{ion}}(\nu) \approx 1.6 \times 10^{-18} (\frac{\nu}{\nu_1}) $, where $\nu_1$ is the frequency corresponding to 13.6 eV. Then the photoionization rate per atom is $ \phi = \int_{\nu_1}^{\infty} \frac{4\pi J(\nu)}{h\nu} \sigma_{\text{ion}}(\nu) d\nu $. The recombination rate to level i is given by $n_e \alpha_i(T) = \int v \sigma_{\text{rec},i} f(v) dv $. The photoionization equilibrium(PIE) is given by $n_e n_{HII} \alpha(T) = n_{HI} \phi$. More generally, $R_i = \frac{\partial n_i}{\partial t} = n_i (n_{i+1} \alpha_{i+1} + n_{i-1} C_{i-1} - n_i (\alpha_i + C_i)) + (n_{i-1} \phi_{i-1} - n_{i} \phi_{i}) $. Then we define the ionization state by $x = \frac{n_{HII}}{n}$, where $n$ is the total number density of hydrogen. Then we can get the equation for the ionization state, which is given by $\frac{1-x}{x^2} = \frac{n \alpha(T)}{\phi}$, and we need to solve this equation. Before we really solve this equation, we can first observe the structure of this equation. For the region close to the star, the photoionization rate is very high, so $\frac{n \alpha}{\phi} \ll 1$, thus we have $ 1-x \ll 1 $. For the region far from the star, the photoionization rate is very low, so $\frac{n \alpha}{\phi} \gg 1$, thus we have $x \ll 1$. So where does the neutral transition occur? We need to bring back the concept of optical depth, which is given by $\tau(\nu,r) = \int_0^r n (1-x) \sigma_{\text{ion}}(\nu) dr' \approx n(1-x) \sigma_{\text{ion}}(\nu) r $, we assume $n \approx const$ and $ 1-x \approx 0 \approx const$ here. The local intensity is given by $u(\nu,r) = \frac{J(\nu,r)}{c}$, the we substitue $J(\nu,r)$ and $\tau(\nu,r)$ into the equation $J(\nu,r) \approx \frac{L_\nu}{4\pi r^2} e^{- \tau(\nu,r)}$ and get $u(\nu,r) \approx \frac{L_\nu}{4\pi r^2 c} e^{- n (1-x) \sigma_{\text{ion}}(\nu) r}$. We get the equation $\frac{d S(r)}{dr} = - 4 \pi r^2 \alpha(T) n^2 x^2$, where $S(r) = \int_{\nu_1}^{\infty} \frac{L_\nu}{h\nu} e^{- n (1-x) \sigma_{\text{ion}}(\nu) r} d\nu$ is the number of ionizing photons per unit time that can reach the radius r. If we assume the density of ionized gas is constant, we can get the Strömgren radius, which is given by $R_S = (\frac{3 S(0)}{4 \pi \alpha(T) n^2})^{1/3}$. The Strömgren radius is the radius at which $S -> 0$. There is no dependence on the cross section and only depends on the total number of ionizing photons, not their energy or cross section. The Strömgren radius is the radius where the ionization and recombination are balanced. 


The second part is about the thermal structure of the HII region. 

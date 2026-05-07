<center> <font size=6>ISM Note 11</font></center>
<center><font size=4>Yang Chen</center>
<center><font size=4>5/7/2026</center>


# Riemann problem


The equation we need to solve is the following:

$$\frac{\partial u}{\partial t} + \nabla \cdot F(u) = 0$$

And the initial condition is:

$$u(x,0) = \begin{cases} u_L, & x < 0 \\ u_R, & x \geq 0 \end{cases}$$

This problem is important for astrophysical simulations, since we need to discretize the continuous fluid into finite volumes, and the Riemann problem occurs at every interface between two adjacent cells. The problem we need to solve here is called the sod shock tube problem, which is a special case of the Riemann problem. The solution to this problem consists of three waves: a shock wave, a contact discontinuity, and a rarefaction wave. The shock wave is a discontinuity in the fluid properties that propagates through the medium, while the contact discontinuity is a surface across which the fluid properties are continuous but the density is not. The rarefaction wave is a smooth expansion wave that propagates through the medium. One sketch of the solution is shown in the figure below:

<figure><style="text-align: center;">
    <img src="" alt="Sod shock tube solution" width="300">
    <figcaption>Fig 1. Sketch of the solution to the sod shock tube problem. The blue line represents the shock wave, the red line represents the contact discontinuity, and the green line represents the rarefaction wave.</figcaption>
</figure>


## Passive Scalar

The passive scalar is a quantity that is advected by the fluid flow but does not affect the dynamics of the fluid, it just evolves with the fluid. This is one thing we can use to dye the fluid.


# Dimensional Analysis


The basic assumption for dimensional analysis is that the dimension function is always a power law. The goal is to get the function form of the solution, e.g. 

$$ a = f(a_1, a_2, ... , a_k, b_1, b_2, ... , b_m) $$

where $a$ is the quantity we want to solve for, $a_i$ are the variables have independent dimensions, and $b_i$ are the dependent variables. So we have

$$ [b_i] = [a_1]^{p_i} [a_2]^{q_i} ... [a_k]^{r_i} $$

and

$$ [a] = [a_1]^{p} [a_2]^{q} ... [a_k]^{r} $$

Here $n = k + m$ is the governing parameters, and $k$ is the number of independent dimensions. Now introduce the dimensionless parameters, which are given by

$$ \Pi = \frac{a}{a_1^p a_2^q ... a_k^r} $$

$$ \Pi_i = \frac{b_i}{a_1^{p_i} a_2^{q_i} ... a_k^{r_i}} $$

If we plug these dimensionless parameters into the original function, we can rewrite the original function as

$$ \Pi = \frac{1}{a_1^p a_2^q ... a_k^r} f(a_1, a_2, ... , a_k, \Pi_1 a_1^{p_1} a_2^{q_1} ... a_k^{r_1}, \Pi_2 a_1^{p_2} a_2^{q_2} ... a_k^{r_2}, ... , \Pi_m a_1^{p_m} a_2^{q_m} ... a_k^{r_m}) $$

And we can define a new function to simplify the above equation, which is given by

$$ \Pi = F(a_1, a_2, ... , a_k, \Pi_1, \Pi_2, ... , \Pi_m) $$

The key thing is, for any $a_i$ with independent dimensions, changed by an arbitrary factor $\lambda$, we can always pass in a unit system to keep $a_2$ ... $a_k$ unchanged. This means the physics does not depend on the choice of the unit system. Therefore this implies that F is independent of $a_i$ ! So we drop out all the $a_i$ in the above equation, and we can get

$$ \Pi = \Phi(\Pi_1, \Pi_2, ... , \Pi_m) $$

So we decrease the dimensions from $n$ to $m= n-k$. Therefore we can rewrite the original function as

$$ f(a_1, a_2, ... , a_k, b_1, b_2, ... , b_m) = a_1^p a_2^q ... a_k^r \Phi(\Pi_1, \Pi_2, ... , \Pi_m) $$

This is the so-called Buckingham Pi theorem, which is a key result in dimensional analysis. For example, we can apply the dimensional analysis to the problem of hydrodynamic drag in a long pipe. We need to solve for the pressure gradient across the cross section of the pipe $\frac{d P}{dx}$, we can write it like

$$ \frac{d P}{dx} = f(\rho, \mu, D, u) $$

And the independent variables are only 3, we can choose them as $u$, $D$, and $\rho$, then we can get

$$ [\frac{d P}{dx}] = [u]^2 [D]^{-1} [\rho] $$

$$ [\mu] = [u] [D] [\rho] $$

Then we can get the dimensionless parameters, which are given by

$$ \Pi = \frac{\frac{d P}{dx}}{u^2 D^{-1} \rho} $$

$$ \Pi_1 = \frac{\mu}{u D \rho} $$

Then we can rewrite the original function as

$$ \frac{d P}{dx} = u^2 D^{-1} \rho \Phi(\frac{\mu}{u D \rho}) $$

So with dimensional analysis, we simplify the original function and get the solution in a more compact form. The experiment gives the relation plot between $\Pi$ and $\Pi_1^{-1}$, which is shown in the figure below:

<figure><style="text-align: center;">
    <img src="" alt="Drag coefficient vs Reynolds number" width="300">
    <figcaption>Fig 2. The relation between the drag coefficient and the Reynolds number.</figcaption>
</figure>

The left smooth curve represents the laminar flow, and the right smooth curve represents the turbulent flow. The transition between these two curves is quite random and it is called the transition flow. The inverse of $\Pi_1$ is called the Reynolds number, which is given by $Re = \frac{u D \rho}{\mu}$. And we can find from this plot that the transition from laminar flow to turbulent flow occurs at $Re \sim 10^3$. 


## The turbulent flow

Also consider the long pipe with a turbulent flow. We impose a pressure difference $P$ between the two ends of the pipe, and we wait for some time $\tau$ then we measure the volume of fluid dropped out from the pipe $Q$, the question is, how does $P$ depend on these parameters? We can write it like

$$ P = f(\tau, Q, \mu, \rho) $$

The independent variables are only 3 as well, and we can choose them as $\tau$, $Q$, and $\mu$, then we can get

$$ [P] = [\tau]^{-1} [Q]^0 [\mu] $$

$$ [\rho] = [\tau] [Q]^{- \frac{2}{3}} [\mu] $$

Then we can get the dimensionless parameters, which are given by

$$ \Pi = \frac{P}{\mu \tau^{-1}} $$

$$ \Pi_1 = \frac{\rho}{\mu \tau Q^{- \frac{2}{3}}} $$

Then we can rewrite the original function as

## Taylor-Sedov blast wave

Assume ambient pressure is negligible, and we want to find the radius of the blast wave as a function of time. Firsr we need to write down the governing parameters, which are given by $t$, $E$, and $\rho$. Then we can get the dimensionless parameter, which is given by


$$ \Pi = \frac{R}{(E t^2 / \rho)^{1/5}} $$

Then we can rewrite the original function as

$$ R = (E t^2 / \rho)^{1/5} \cdot const $$

Sedov is the energy conserving phase of SNR. The system is self-similar, which means the solution at different time is the same, just with a different scale. (This needs to be explained more clearly)


## Supernova remnant (SNR)

The first is the Sedov phase, which is the energy conserving phase. For this phase, we have for the dynamic timescale $t_{dyn} \ll t_{cool}$, so the cooling is negligible. The energy can be given by

$$ e = \frac{1}{2} v^2 = \frac{9}{32} \dot{R}^2 $$

The coefficient $\frac{9}{32}$ comes from the shock jump condition. And since the kinetic energy is comparable to the internal energy, so that the total energy is given by

$$ E_{total} = \frac{4 \pi}{3} R^3 \rho_0 (e + \frac{1}{2} v^2) = \frac{4 \pi}{3} \rho_0 R^3 \dot{R}^2 = E_{SN} $$


So we can solve for $R(t)$ from the equation above, and we can get

$$ R(t) = \left ( \frac{25}{3 \pi}  \right )^{1/5}  \left ( \frac{E_{SN} t^2}{\rho_0} \right )^{1/5} $$

And $v(t) = \dot{R}(t)$ as below

$$ v(t) = \frac{2}{5} \left ( \frac{25}{3 \pi}  \right )^{1/5}  \left ( \frac{E_{SN}}{\rho_0 t^3} \right )^{1/5} $$


The second is the snowplow phase, which is the momentum conserving phase. For this phase, we have 

$$ M_{shell}(t) \dot{R}(t) \sim R^3 \rho_0 \dot{R}(t) \sim R^3 \frac{d R}{dt} = const $$

And then we can get 

$$ R(t) \propto t^{1/4} $$

$$ v(t) \propto t^{-3/4} $$






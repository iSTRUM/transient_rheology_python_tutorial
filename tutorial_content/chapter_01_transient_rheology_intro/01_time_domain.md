# the time domain 

The modulus, $M(t)$, describes the response of a rock to an applied stress. In the purely elastic 
case, the modulus is anologous to the spring constant of a spring: given an applied stress, a spring stretches 
effectively instananeously to a length determined by the spring constant. In the case of 
a transient rheology, the modulus is a time dependent function, $M(t)$. Rather than working with the 
modulus, $M$, however, it is common to instead think in terms of the **compliance**, which is the inverse of the modulus:

$$
J(t) = \frac{1}{M(t)} 
$$

The time dependence of deformation can be described by what is commonly called the creep function, 

$$
J(t) = J_u + \Gamma(t) + \frac{t}{\eta_{ss}}
$$

where $J_u$ is the unrelaxed (purely elastic) compliance, $\Gamma(t)$ is a to-be-determined function that 
describes the time dependent evolution and $eta_{ss}$ is the effective steady state viscosity of the material.
With a bit of algebra this can also be written 

$$
J(t) = J_u \left (1 + \Gamma'(t) + \frac{t}{J_u \eta_{ss}} \right)
$$

The term $J_u \eta_{ss}$ can be recognized as the characteristic Maxwell time, 

$$
\tau_M = \frac{\eta_{ss}}{M_u} = J_u \eta_{ss} 
$$

And we can write the creep function instead as 

$$
J(t) = J_u \left (1 + \Gamma'(t) + \frac{t}{\tau_m} \right)
$$

For 

$$
J(t) / J_u = \left (1 + \Gamma'(t) + \frac{t}{\tau_m} \right)
$$


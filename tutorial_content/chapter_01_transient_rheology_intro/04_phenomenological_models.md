# models of viscoelasticity and transient deformation

Up to this point, we've been talking in pretty general terms about time dependent deformation. The creep function describes the time dependent response, attenuation is the lag between stress and strain curves, under cyclical loading we can re-cast the time dependence as a frequency dependence. But to answer interesting questions related to material response or to apply our understanding of deformation to a wide range of conditions, we need a more careful description for the creep function, $J(t)$. In particular, we are interested in answering the question what are the physical processes and parameters that control a material's creep function? And how does the thermodynamic state (the temperature, pressure, grain size, composition, etc.) influence the creep function? Answering these questions let's us apply our understanding materials properties to a wide range of geophysics and ask questions that are fundamental to our understanding of deformation across spatio-temporal scales from global plate tectonics, to glacial-isostatic adjustment to post-seismic deformation.

Refining the formulation of $J(t)$ relies heavily on deformation experiments. In general, these experiments produce stress and strain curves (and possibly attenuation measurements if using cyclical loads) at a range of conditions (load amplitude, temperature, composition, etc.). The results can then be used to test models of deformation: for example...

While a full physics-based model can offer additional insight, it is often simplify deformation models in terms of a collection of interacting viscous and elastic responses. This gives rise to the so-called "phenomenological models". The basic building blocks of the phenomenological models are the pure elastic and pure viscous endmembers.



Pure elastic endmember: hooke's law with spring constant. Given an applied stress, instantaneous elastic response. Represented with a spring:


```
\/\/\/\/
```

Pure viscous endmember: given an applied stress, the material deforms with an effective viscosity. Represented by a dashpot. What's a dashpot?

DASHPOT PHOTO

```
  _____
  | |
--| |------
  |_|__
```

From here, we can connect our endmember in near-endless configurations to capture a range of responses.

### The Phenomenological Models

## Hooke Model

A purely elastic response

$$
J(t) = J_u
$$

## Newton Model

A purely viscous response

$$
J(t) = t / \eta
$$

## Voigt-Kelvin

A Hooke and Newton model in parallel. On application of stress, there is no instantaneous elastic response: the material will flow until the elastic component balances the applied stress.

$$
J(t) = J_u (1 - \mathrm{exp}(- t / \tau_m))
$$

## Maxwell Model

Hooke model and Newton model in series

$$
J(t) = J_u + t / \eta
$$

Or, with the definition of $\tau_m$ as the characteristic maxwell time, $\tau_m = \eta_{ss} J_u = \eta{ss} / G_u$,

$$
J(t) = J_u (1 + t / \tau_m)
$$

## Standard Linear Solid

Voigt-Kelvin in series with a Hooke model. On application of stress, there is an instaneous elastic reponse, followed by a time-dependent additional relaxation:

$$
J(t) = J_{u1} + J_{u2} (1 - \mathrm{mathrm}(-t/\tau_{m2}))
$$

## Burgers Model

The Burgers model: the most general of the simple models, the Burgers model is a Voigt-Kelvin element in series with a  Maxwell element (or, an SLS with a Newton dashpot):

$$
J(t) = J_{u1} (1 + t/\tau_{m1}) + J_{u2} (1 - \mathrm{mathrm}(-t/\tau_{m2}))
$$


## Andrade Model

A semi-empirical power law formulation
$$
J(t) = J_u (1 + t/\tau_m) + \Beta t^\alpha
$$

## Extended models

Superposition!

Generalized polynomial relaxation specturm (e.g., Takei et al)

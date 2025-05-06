# The Phenomenal Phenomenological Models 

Up until this point, we've been talking in very general terms -- the creep function describes the time dependent response to deformation, but how do we **calculate** it? In defomration experiments, researchers do stuff... 



## Maxwell Model

When $\Gamma'(t)=0$, 

```python
from sympy import symbols
from sympy.plotting import plot
import unyt
t = symbols('t')
tau_m_values = unyt.unyt_array([1e3, 1e4, 1e5], 'years').to('s')
plots = []
for tau_m in tau_m_values:
    J_t = 1 + t / tau_m
    plots.append(plot(J_t, show=False))

for itau in range(2, len(tau_m_values)):
    plots[0].append(plots[itau][0])
plots[0]    
plots[0].show()
```

## Andrade Model 

## Burgers Model 

## Zener Model

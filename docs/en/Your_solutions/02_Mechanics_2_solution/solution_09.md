## 9. Vertical Throw with Drag (Differential Equations)

### Problem Statement
A particle of mass $m$ is thrown vertically with an initial velocity $v(0) = v_0$ from an initial height $x(0) = 10$. The equation of motion, including linear air drag, is:
$$m \frac{dv}{dt} = -mg - kv$$
1. Solve the equation analytically for $v(t)$.
2. Determine the maximum height reached.
3. Compare the result with the case without drag.
4. Perform a numerical simulation.

---

### Analytical Solution

#### 1. Solving for Velocity $v(t)$
We rewrite the equation as a first-order linear differential equation:
$$\frac{dv}{dt} + \frac{k}{m}v = -g$$

Using the integrating factor $e^{\int (k/m) dt} = e^{(k/m)t}$, or by separating variables:
$$\frac{dv}{v + \frac{mg}{k}} = -\frac{k}{m} dt$$

Integrating both sides and applying the initial condition $v(0) = v_0$:
$$v(t) = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m}t} - \frac{mg}{k}$$

#### 2. Maximum Height
The particle reaches maximum height when $v(t) = 0$. Solving for $t_{max}$:
$$0 = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m}t_{max}} - \frac{mg}{k} \implies t_{max} = \frac{m}{k} \ln\left( 1 + \frac{kv_0}{mg} \right)$$

Integrating $v(t)$ to find $x(t)$ and substituting $t_{max}$ gives the maximum height.

#### 3. Comparison with Vacuum Case ($k=0$)
- **With Drag:** The acceleration is always greater (in magnitude) than $g$ during ascent, meaning the particle reaches a **lower** maximum height in a **shorter** time.
- **Terminal Velocity:** Unlike the vacuum case, the particle with drag eventually reaches a constant terminal velocity $v_t = -\frac{mg}{k}$.

#### 4. Numerical Simulation (Python)
```python
import numpy as np
from scipy.integrate import odeint

def model(v, t, m, g, k):
    return -g - (k/m)*v

# Constants
m, g, k, v0 = 1.0, 9.81, 0.1, 20.0

## 9. Vertical Throw with Drag (Differential Equations)

### Problem Statement
A particle of mass $m$ is thrown vertically upward with an initial velocity $v(0) = v_0$. The motion is affected by gravity and a linear air resistance force $F_d = -kv$.
The equation of motion is:
$$m \frac{dv}{dt} = -mg - kv$$

1. Derive the analytical expression for velocity $v(t)$.
2. Calculate the time to reach maximum height ($t_{up}$).
3. Discuss the concept of **Terminal Velocity** ($v_t$).

---

### Analytical Solution

#### 1. Solving the Differential Equation
We can rewrite the equation of motion as:
$$\frac{dv}{dt} + \frac{k}{m}v = -g$$

This is a first-order linear differential equation. Using an integrating factor $e^{(k/m)t}$ or by separating variables:
$$\int_{v_0}^{v(t)} \frac{dv}{g + \frac{k}{m}v} = -\int_{0}^{t} dt$$

Integrating both sides:
$$\frac{m}{k} \ln\left( \frac{g + \frac{k}{m}v(t)}{g + \frac{k}{m}v_0} \right) = -t$$

Solving for $v(t)$:
$$v(t) = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m}t} - \frac{mg}{k}$$

#### 2. Time to Maximum Height ($t_{up}$)
At maximum height, the instantaneous velocity is zero ($v(t_{up}) = 0$):
$$0 = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m}t_{up}} - \frac{mg}{k}$$
$$e^{\frac{k}{m}t_{up}} = 1 + \frac{kv_0}{mg}$$
$$t_{up} = \frac{m}{k} \ln\left( 1 + \frac{kv_0}{mg} \right)$$

#### 3. Terminal Velocity ($v_t$)
As the particle falls back down ($t \to \infty$), the acceleration becomes zero. The forces of gravity and air drag balance each other:
$$-mg - kv_t = 0 \implies v_t = -\frac{mg}{k}$$
The velocity approaches this constant value regardless of the starting height, provided the fall is long enough.

---

### Comparison: Vacuum vs. Air Drag
| Feature | Vacuum ($k=0$) | Air Drag ($k>0$) |
| :--- | :--- | :--- |
| **Acceleration** | Constant ($-g$) | Variable ($-g - \frac{k}{m}v$) |
| **Max Height** | Higher | Lower |
| **Velocity Curve** | Linear | Exponential |
| **Final Speed** | Increases indefinitely | Limits at $v_t$ |

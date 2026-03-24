# 9. Vertical Throw with Air Resistance (Analytical Solution)

This problem explores the dynamics of a particle thrown vertically upward in a medium where air resistance is proportional to its velocity ($F_d = -kv$).

---

### 1. Problem Statement
A particle of mass $m$ is launched vertically upward with an initial velocity $v(0) = v_0$. The forces acting on the particle are gravity ($mg$) and linear air drag ($kv$). 

Find:
1. The equation of motion.
2. The velocity as a function of time $v(t)$.
3. The time required to reach the maximum height $t_{up}$.
4. The terminal velocity $v_t$.

---

### 2. Derivation of the Equation of Motion
According to Newton's Second Law ($F = ma$), the sum of forces in the vertical direction (taking upward as positive) is:
$$m \frac{dv}{dt} = -mg - kv$$

To solve for $v(t)$, we rearrange the equation into a separable form:
$$\frac{dv}{g + \frac{k}{m}v} = -dt$$

---

### 3. Solving for Velocity $v(t)$
Integrating both sides from $t=0$ (where $v=v_0$) to a general time $t$ (where velocity is $v$):
$$\int_{v_0}^{v} \frac{dv}{g + \frac{k}{m}v} = \int_{0}^{t} -dt$$

The integral of the left side involves a natural logarithm:
$$\frac{m}{k} \left[ \ln\left( g + \frac{k}{m}v \right) \right]_{v_0}^{v} = -t$$
$$\ln\left( \frac{g + \frac{k}{m}v}{g + \frac{k}{m}v_0} \right) = -\frac{k}{m}t$$

Taking the exponential of both sides and isolating $v$:
$$v(t) = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m}t} - \frac{mg}{k}$$



---

### 4. Time to Reach Maximum Height ($t_{up}$)
The particle reaches its peak when the instantaneous velocity is zero ($v(t_{up}) = 0$):
$$0 = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m}t_{up}} - \frac{mg}{k}$$
$$\frac{mg}{k} = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m}t_{up}}$$
$$e^{\frac{k}{m}t_{up}} = \frac{v_0 + \frac{mg}{k}}{\frac{mg}{k}} = 1 + \frac{kv_0}{mg}$$

Taking the natural logarithm:
$$t_{up} = \frac{m}{k} \ln\left( 1 + \frac{kv_0}{mg} \right)$$

---

### 5. Terminal Velocity ($v_t$)
As the particle falls back down and $t \to \infty$, the velocity approaches a constant value where the upward drag force equals the downward gravitational force:
$$v_t = \lim_{t \to \infty} v(t) = -\frac{mg}{k}$$
The negative sign indicates the direction of motion is downward.

---

### 6. Comparison Table
| Property | Vacuum (Ideal) | With Air Drag (Real) |
| :--- | :--- | :--- |
| **Acceleration** | Constant ($-g$) | Decreases as velocity drops |
| **Velocity Profile** | Linear ($v_0 - gt$) | Exponential Decay |
| **Max Height** | Higher ($v_0^2 / 2g$) | Lower (Energy lost to heat) |
| **Symmetry** | Symmetric (Time up = Time down) | Asymmetric (Time down > Time up) |

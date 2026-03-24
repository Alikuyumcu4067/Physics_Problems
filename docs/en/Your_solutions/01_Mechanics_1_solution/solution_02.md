## 2. Range Optimization (Projectile Motion)

### Problem Statement
For a projectile launched with an initial velocity $v_0$ at an angle $\theta$ above the horizontal, show analytically that the maximum horizontal range $R(\theta)$ is achieved at a launch angle of **$45^\circ$**.

Assume the range formula is given by:
$$R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$$

---

### Analytical Proof

To find the angle $\theta$ that maximizes the range $R$, we must find the derivative of $R$ with respect to $\theta$ and set it to zero ($\frac{dR}{d\theta} = 0$).

#### Step 1: Differentiation
The parameters $v_0$ and $g$ (gravitational acceleration) are constants. We apply the derivative to the trigonometric function:
$$\frac{dR}{d\theta} = \frac{d}{d\theta} \left[ \frac{v_0^2 \sin(2\theta)}{g} \right]$$
$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot \frac{d}{d\theta}(\sin(2\theta))$$

Using the **chain rule** ($\frac{d}{dx}\sin(u) = \cos(u) \cdot \frac{du}{dx}$):
$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot 2\cos(2\theta)$$

#### Step 2: Setting to Zero
To find the extremum (maximum), set the derivative to zero:
$$\frac{2v_0^2}{g} \cos(2\theta) = 0$$

Since $\frac{2v_0^2}{g} \neq 0$, we must have:
$$\cos(2\theta) = 0$$

#### Step 3: Solving for $\theta$
The cosine function is zero at $90^\circ$ (or $\pi/2$ radians) for the primary range of projectile motion:
$$2\theta = 90^\circ$$
$$\mathbf{\theta = 45^\circ}$$

---

### Physical Interpretation
- **At $45^\circ$:** The term $\sin(2\theta)$ reaches its maximum value of $1$. This balances the trade-off between vertical flight time and horizontal velocity perfectly.
- **Complementary Angles:** Note that angles symmetric around $45^\circ$ (e.g., $30^\circ$ and $60^\circ$) result in the same range because $\sin(2 \cdot 30^\circ) = \sin(2 \cdot 60^\circ) = \sin(120^\circ)$.
- **Maximum Value:** The maximum range is simply $R_{max} = \frac{v_0^2}{g}$.

> **Note:** This proof assumes no air resistance. In real-world conditions with air drag, the optimal angle is typically slightly less than $45^\circ$ (around $35^\circ$-$42^\circ$ depending on the object).

## 2. Range Optimization (Projectile Motion)

### Problem Statement
For a projectile launched with an initial velocity $v_0$ at an angle $\theta$ above the horizontal, show analytically that the maximum horizontal range $R(\theta)$ is achieved at a launch angle of **$45^\circ$**.

The horizontal range formula is given by:
$$R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$$

---

### Analytical Proof

To find the angle $\theta$ that maximizes the range $R$, we seek the critical point where the first derivative of $R$ with respect to $\theta$ is zero:
$$\frac{dR}{d\theta} = 0$$

#### Step 1: Differentiation
Since $v_0$ and $g$ are constant for a given launch, we differentiate the trigonometric function:
$$\frac{dR}{d\theta} = \frac{d}{d\theta} \left[ \frac{v_0^2 \sin(2\theta)}{g} \right]$$
$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot \frac{d}{d\theta}(\sin(2\theta))$$

Using the **chain rule** ($\frac{d}{dx}\sin(ax) = a\cos(ax)$):
$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot 2\cos(2\theta)$$

#### Step 2: Finding the Maximum
To find the maximum range, set the derivative to zero:
$$\frac{2v_0^2}{g} \cos(2\theta) = 0$$

Since $\frac{2v_0^2}{g}$ is a non-zero constant, we solve for:
$$\cos(2\theta) = 0$$

#### Step 3: Solving for $\theta$
The cosine function equals zero when its argument is $90^\circ$ (or $\pi/2$ radians):
$$2\theta = 90^\circ$$
$$\mathbf{\theta = 45^\circ}$$

---

### Physical Interpretation
- **Optimization:** At $45^\circ$, the term $\sin(2\theta)$ becomes $\sin(90^\circ) = 1$, which is the maximum possible value for the sine function.
- **Maximum Range Formula:** Substituting $\theta = 45^\circ$ back into the original equation gives:
  $$R_{max} = \frac{v_0^2}{g}$$
- **Symmetry:** Projectiles launched at complementary angles (e.g., $30^\circ$ and $60^\circ$) will land at the same spot because $\sin(2\theta)$ yields the same value for both.

> **Note:** This analytical model assumes a vacuum. In real-world physics with air resistance (drag), the optimal angle for maximum distance is typically slightly lower than $45^\circ$.

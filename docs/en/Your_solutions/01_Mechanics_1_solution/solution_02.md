# Solution 2: Range Optimization

## Problem Statement
For projectile motion, show analytically that the maximum range $R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$ for a given initial velocity is achieved at a launch angle of $45^\circ$.

---

## Analytical Proof

The horizontal range $R$ is given as a function of the launch angle $\theta$:
$$R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$$

To find the angle $\theta$ that maximizes the range, we take the first derivative of $R$ with respect to $\theta$ and set it to zero ($\frac{dR}{d\theta} = 0$).

### 1. Differentiation
Using the chain rule for $\sin(2\theta)$:
$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot \frac{d}{d\theta}(\sin 2\theta)$$
$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot (2 \cos 2\theta)$$

### 2. Finding the Critical Point
Set the derivative to zero to find the maximum:
$$\frac{2 v_0^2 \cos 2\theta}{g} = 0$$

Since $v_0$ and $g$ are constant positive values, the equation holds true only if:
$$\cos(2\theta) = 0$$

### 3. Solving for $\theta$
The cosine function equals zero when the angle is $90^\circ$ (within the physical limits of projectile motion):
$$2\theta = 90^\circ$$
$$\theta = 45^\circ$$

### 4. Conclusion
At $\theta = 45^\circ$, the term $\sin(2\theta) = \sin(90^\circ) = 1$, which is the maximum possible value for the sine function. Therefore, the maximum range is achieved at a launch angle of **$45^\circ$**.


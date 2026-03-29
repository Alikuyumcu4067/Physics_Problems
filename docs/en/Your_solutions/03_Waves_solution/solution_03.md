## 3. Superposition Principle

**Problem:**
Two waves are described by the equations $y_1(x, t) = A \sin(kx - \omega t)$ and $y_2(x, t) = A \sin(kx + \omega t)$. 
1. What is the equation of the resulting standing wave? 
2. Identify the positions of the nodes.

**Solution:**

### 3.1. Resulting Standing Wave Equation
According to the **Principle of Superposition**, the resultant displacement $y(x, t)$ is the sum of the two individual waves:
$$y(x, t) = y_1 + y_2 = A \sin(kx - \omega t) + A \sin(kx + \omega t)$$

Using the trigonometric identity $\sin(\alpha - \beta) + \sin(\alpha + \beta) = 2 \sin \alpha \cos \beta$, where $\alpha = kx$ and $\beta = \omega t$:
$$y(x, t) = 2A \sin(kx) \cos(\omega t)$$

### 3.2. Identifying Node Positions
**Nodes** are points where the displacement is always zero ($y = 0$). This occurs when the spatial part of the equation, $\sin(kx)$, is zero:
$$\sin(kx) = 0$$

This happens when the argument $kx$ is an integer multiple of $\pi$:
$$kx = n\pi \quad \text{where } n = 0, 1, 2, \dots$$

Since $k = \frac{2\pi}{\lambda}$, we can solve for $x$:
$$\left(\frac{2\pi}{\lambda}\right)x = n\pi$$
$$x = \frac{n\lambda}{2}$$

**Answer:** The nodes are located at positions $x = 0, \frac{\lambda}{2}, \lambda, \frac{3\lambda}{2}, \dots$ (every half-wavelength).

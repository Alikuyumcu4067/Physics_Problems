## 3. Superposition Principle – Detailed Step-by-Step Solution

### **Problem Statement**
Two waves traveling in opposite directions are described by the equations:
1. $y_1(x,t) = A \sin(kx - \omega t)$  *(Wave traveling to the right)*
2. $y_2(x,t) = A \sin(kx + \omega t)$  *(Wave traveling to the left)*

**Task:**
* Derive the equation of the resulting **standing wave**.
* Determine the exact positions of the **nodes** (points of zero displacement).

---

### **Step 1: Application of the Superposition Principle**
The principle of superposition states that the resultant displacement of a medium is the algebraic sum of the displacements of the individual waves.
$$y_{total}(x,t) = y_1(x,t) + y_2(x,t)$$

Substituting the given wave functions:
$$y(x,t) = A \sin(kx - \omega t) + A \sin(kx + \omega t)$$

---

### **Step 2: Trigonometric Derivation (The Proof)**
To combine these two sine functions, we apply the trigonometric sum-to-product identity:
$$\sin(\alpha) + \sin(\beta) = 2 \sin\left(\frac{\alpha + \beta}{2}\right) \cos\left(\frac{\alpha - \beta}{2}\right)$$

Let **$\alpha = kx + \omega t$** and **$\beta = kx - \omega t$**:
* **Average of arguments:** $\frac{\alpha + \beta}{2} = \frac{(kx + \omega t) + (kx - \omega t)}{2} = \frac{2kx}{2} = kx$
* **Half-difference of arguments:** $\frac{\alpha - \beta}{2} = \frac{(kx + \omega t) - (kx - \omega t)}{2} = \frac{2\omega t}{2} = \omega t$

Plugging these back into the identity, we get the standing wave equation:
$$y(x,t) = \mathbf{2A \sin(kx) \cos(\omega t)}$$

---

### **Step 3: Finding the Positions of the Nodes**
**Nodes** are fixed points in space ($x$) where the displacement is zero for all time ($t$). This occurs when the spatial part of the equation ($2A \sin(kx)$) is zero:
$$\sin(kx) = 0$$

The sine function is zero at integer multiples of $\pi$:
$$kx = n\pi \quad \text{where } n = 0, 1, 2, 3, \dots$$

---

### **Step 4: Expressing Nodes in Terms of Wavelength ($\lambda$)**
Since the wave number $k$ is defined as $k = \frac{2\pi}{\lambda}$, we substitute this into the node condition:
$$\left( \frac{2\pi}{\lambda} \right) x = n\pi$$

Solving for $x$:
1. Divide both sides by $\pi$: $\frac{2x}{\lambda} = n$
2. Isolate $x$:
$$x = n \frac{\lambda}{2} \quad (n = 0, 1, 2, 3, \dots)$$

---

### **Step 5: Final Results Summary**

| Category | Mathematical Expression |
| :--- | :--- |
| **Resultant Wave Equation** | $y(x,t) = \mathbf{2A \sin(kx) \cos(\omega t)}$ |
| **Node Positions ($x$)** | $x = \mathbf{0, \frac{\lambda}{2}, \lambda, \frac{3\lambda}{2}, \dots}$ |
| **Antinode Positions ($x$)** | $x = \frac{\lambda}{4}, \frac{3\lambda}{4}, \frac{5\lambda}{4}, \dots$ |

---

### **Step 6: Physical Analysis**
1.  **Nature of the Wave:** The separation of the spatial term $\sin(kx)$ and the temporal term $\cos(\omega t)$ confirms this is a **standing wave**. It does not "travel" through space; instead, the medium oscillates in a fixed pattern.
2.  **Amplitude:** The maximum amplitude at the antinodes is $2A$, which is twice the amplitude of the individual traveling waves.
3.  **Nodes:** These are points of complete destructive interference. At $x = n\lambda/2$, the string (or medium) remains completely stationary.

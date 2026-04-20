# 🔬 Advanced Electromagnetism: Biot-Savart Analysis

## Case Study 3: Magnetic Field of a Discrete Current Segment

### 📌 Problem Overview
Calculating the magnetic flux density ($B$) at a specific point $P$ induced by a $0.1\text{ m}$ wire segment carrying a $3\text{ A}$ current at a distance of $0.2\text{ m}$.

---

### 📥 Input Parameters
| Variable | Notation | Value |
| :--- | :--- | :--- |
| Current | $I$ | $3\text{ A}$ |
| Segment Length | $\Delta L$ | $0.1\text{ m}$ |
| Distance | $r$ | $0.2\text{ m}$ |
| Vacuum Permeability | $\mu_0/4\pi$ | $10^{-7} \text{ T}\cdot\text{m/A}$ |

---

### ⚙️ Derivation & Solution Steps

#### 1. Fundamental Formula
We utilize the **Biot-Savart Law** magnitude formula for a finite segment:
$$B = \frac{\mu_0}{4\pi} \frac{I \Delta L \sin \theta}{r^2}$$

#### 2. Angular Simplification
Given that the segment is perpendicular to the position vector:
$$\theta = 90^\circ \implies \sin(90^\circ) = 1$$

#### 3. Numerical Substitution
Substituting the parameters into the equation:
$$B = 10^{-7} \times \frac{3 \times 0.1 \times 1}{(0.2)^2}$$

#### 4. Final Computation
- **Source Strength ($I \cdot \Delta L$):** $0.3\text{ A}\cdot\text{m}$
- **Spatial Decay ($r^2$):** $0.04\text{ m}^2$
- **Total Field:** $B = 10^{-7} \times 7.5 = 7.5 \times 10^{-7}\text{ T}$

---

### 💡 Presentation Strategy (Defense Notes)
* **Why not Ampere's Law?** Ampere's Law is best for high-symmetry infinite systems. For a **finite segment** like this, Biot-Savart is the only accurate method.
* **Inverse Square Dependency:** Emphasize that the field strength drops by $1/r^2$. This shows that magnetic effects from small segments vanish very quickly as distance increases.
* **Units:** Always mention the result in **Tesla (T)**. For small values like this, using **microTesla ($\mu$T)** makes the data more readable for the audience.

> [!NOTE]
> This calculation assumes the segment is small enough to be treated as a single element. For much longer wires, an integral across the entire length would be required.

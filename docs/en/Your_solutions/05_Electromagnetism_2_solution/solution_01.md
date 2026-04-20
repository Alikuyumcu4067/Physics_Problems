### 1. Gauss's Law: Quantitative Flux Analysis

**Problem:** Calculation of electric flux ($\Phi_E$) for a $+2\text{ C}$ point charge enclosed by a spherical surface ($r=1\text{ m}$).

#### Mathematical Derivation
The solution utilizes the integral form of **Gauss's Law**. The fundamental principle dictates that the flux is independent of the geometry of the enclosing surface and the distribution of the charge within that volume.

$$\Phi_E = \oint_S \mathbf{E} \cdot d\mathbf{A} = \frac{Q_{\text{enc}}}{\varepsilon_0}$$

#### Parameter Specification
| Parameter | Symbol | Value | Unit |
| :--- | :--- | :--- | :--- |
| Enclosed Charge | $Q_{\text{enc}}$ | $2.0$ | Coulombs (C) |
| Permittivity of Free Space | $\varepsilon_0$ | $8.854 \times 10^{-12}$ | $\text{C}^2/(\text{N}\cdot\text{m}^2)$ |
| Sphere Radius | $r$ | $1.0$ | Meters (m) |

#### Step-by-Step Calculation
1. **Enclosure Verification:** The charge is at the origin $(0,0,0)$, placing it strictly inside the boundary $r=1$.
2. **Numerical Computation:**
   $$\Phi_E = \frac{2}{8.854 \times 10^{-12}}$$
   $$\Phi_E \approx 2.26 \times 10^{11} \text{ V}\cdot\text{m}$$

> [!TIP]
> **Key Insight:** The radius provided in the problem is a spatial parameter that does not influence the net flux. This demonstrates the "Inverse Square Law" cancellation effect inherent in Gauss's Law.

# Section 4: Electromagnetism I - Problem 1

## 1. Coulomb's Law: Electrostatic Force in a Symmetric System

**Problem:** Four point charges of $+1.0 \text{ C}$ each are placed at the corners of a square with sides of $1.0 \text{ m}$. Calculate the magnitude and direction of the electric force on a charge of $-2.0 \text{ C}$ placed at the center of the square.

---

### I. System Geometry
For a square with side length $a = 1.0 \text{ m}$, the distance $r$ from each corner to the center (the circumradius) is calculated using the Pythagorean theorem:
$$d = a\sqrt{2} \implies r = \frac{d}{2} = \frac{a\sqrt{2}}{2}$$
Substituting $a = 1.0$:
$$r = \frac{\sqrt{2}}{2} \approx 0.707 \text{ m}$$

### II. Physical Principles
According to **Coulomb's Law**, the magnitude of the force $F$ between two point charges $Q$ and $q$ is:
$$F = k \frac{|Q \cdot q|}{r^2}$$
* **Nature of the Force:** Since the corner charges are positive ($+1.0 \text{ C}$) and the center charge is negative ($-2.0 \text{ C}$), the force is **attractive**. 
* **Vector Direction:** The center charge is pulled towards each corner along the diagonals.

### III. Vector Superposition Analysis
Let the corners be defined as $A, B, C,$ and $D$ in clockwise order.
1.  **Force from Corner A and C:** These two charges are located at opposite ends of the same diagonal. They both exert an attractive force of equal magnitude on the center charge but in exactly opposite directions.
    $$\vec{F}_A = -\vec{F}_C \implies \vec{F}_A + \vec{F}_C = 0$$
2.  **Force from Corner B and D:** Similarly, these two charges are on the opposite ends of the other diagonal.
    $$\vec{F}_B = -\vec{F}_D \implies \vec{F}_B + \vec{F}_D = 0$$

### IV. Calculation of Net Force
The total net force $\vec{F}_{net}$ is the vector sum of all individual forces:
$$\vec{F}_{net} = \vec{F}_A + \vec{F}_B + \vec{F}_C + \vec{F}_D$$
Using the symmetry observed above:
$$\vec{F}_{net} = (\vec{F}_A + \vec{F}_C) + (\vec{F}_B + \vec{F}_D) = 0 + 0 = 0$$

---

### Final Result
* **Magnitude of Net Force:** $0 \text{ N}$
* **Direction:** None (The system is in a state of unstable electrostatic equilibrium).

**Conclusion:** Due to the perfect symmetry of the charge distribution, the resultant electric force on the central charge is zero.

## 4. Geostationary Orbit (Step-by-Step)

### Part 1: Orbital Period ($T$)
To stay directly over the same point on Earth, a satellite must match Earth's true rotational period (one sidereal day):
* **Period ($T$):** 23 hours, 56 minutes, 4 seconds
* **In Seconds:** $T = 86,164 \text{ s}$

---

### Part 2: Calculation of Orbital Altitude

#### Step 1: Identify Constants
* **Earth's Gravitational Parameter ($G M_E$):** $3.9844 \times 10^{14} \text{ m}^3/\text{s}^2$
* **Earth's Radius ($R_E$):** $6378 \text{ km}$

#### Step 2: Use Kepler's Third Law for Total Orbital Radius ($r$)
$$r = \left( \frac{G M_E T^2}{4\pi^2} \right)^{1/3}$$

Plugging in our parameters:
$$r = \left( \frac{3.9844 \times 10^{14} \times (86,164)^2}{4\pi^2} \right)^{1/3}$$
$$r = \left( \frac{2.958 \times 10^{24}}{39.4784} \right)^{1/3}$$
$$r = (7.4927 \times 10^{22})^{1/3} \approx 42,158,000 \text{ m} \approx 42,158 \text{ km}$$

#### Step 3: Subtract Earth's Radius to Find Altitude ($h$)
$$h = r - R_E$$
$$h = 42,158 \text{ km} - 6378 \text{ km} = 35,780 \text{ km}$$

---

> **Result:** A geostationary satellite must have an orbital period of **23 hours 56 minutes 4 seconds**, orbiting at an altitude of approximately **$35,780 \text{ km}$** above Earth's surface.

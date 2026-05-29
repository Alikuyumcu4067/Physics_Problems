## 10. Measuring the Height of the Atmosphere (Geometric Analysis)

### Step 1: Calculate the Solar Depression Angle ($\phi$)
The angular velocity of Earth's rotation ($\omega$) per minute is defined as:
$$\omega = \frac{360^\circ}{24 \times 60 \text{ min}} = 0.25^\circ/\text{min}$$

Given an observation time interval $t = 40 \text{ minutes}$:
$$\phi = \omega \times t = 0.25^\circ/\text{min} \times 40 \text{ min} = 10^\circ$$

### Step 2: Establish the Tangential Boundary Formula
Using the right-triangle framework of a ray grazing the atmosphere:
$$\cos(\phi) = \frac{R_E}{R_E + h}$$

Isolating the structural height factor ($h$):
$$h = R_E \left( \frac{1}{\cos(\phi)} - 1 \right)$$

### Step 3: Compute Atmospheric Height ($h$)
Substitute the given baseline Earth radius ($R_E = 6370 \text{ km}$) and computed angle ($\phi = 10^\circ$):
$$h = 6370 \times \left( \frac{1}{\cos(10^\circ)} - 1 \right)$$
$$h = 6370 \times \left( \frac{1}{0.984808} - 1 \right)$$
$$h = 6370 \times 0.015427 \approx 98.27 \text{ km}$$

---

> **Conclusion:** The solar depression angle is exactly **$10^\circ$**, yielding an estimated sharp-edge atmospheric boundary height of **$98.27 \text{ km}$**.

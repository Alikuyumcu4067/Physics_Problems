## 1. Propagation of Error I: Volume of a Sphere

The volume $V$ of a sphere is calculated using the formula:
$$V = \frac{4}{3}\pi r^3$$

### Given Data:
* Measured radius ($r$) = $6.20 \text{ cm}$
* Absolute uncertainty in radius ($\delta r$) = $0.05 \text{ cm}$

---

### Step-by-Step Calculation:

#### 1. Calculate the Central Value of the Volume
Substitute the measured radius into the volume formula:
$$V = \frac{4}{3} \pi (6.20)^3$$
$$V = \frac{4}{3} \pi (238.328) \approx 998.306 \text{ cm}^3$$

#### 2. Calculate the Uncertainty Using Error Propagation (Power Rule)
When a variable is raised to a power (i.e., $r^3$), its relative uncertainty is multiplied by the power. The constant $\frac{4}{3}\pi$ has no uncertainty.

The relative uncertainty formula for volume is:
$$\frac{\delta V}{V} = 3 \frac{\delta r}{r}$$

Now, solve for the absolute uncertainty ($\delta V$):
$$\delta V = 3 \cdot \left(\frac{\delta r}{r}\right) \cdot V$$
$$\delta V = 3 \cdot \left(\frac{0.05}{6.20}\right) \cdot 998.306$$
$$\delta V = 3 \cdot 0.0080645 \cdot 998.306 \approx 24.152 \text{ cm}^3$$

---

### Formatting the Final Answer:
Following standard experimental physics rules, the absolute uncertainty should be rounded to **one or two significant figures** (usually one or two depending on precision, let's keep one decimal place to match the precision), and the central value must be rounded to the same decimal place.

* $\delta V \approx 24.2 \text{ cm}^3$
* $V \approx 998.3 \text{ cm}^3$

### Final Result:
The calculated volume of the sphere with its associated uncertainty is:
$$V = (998.3 \pm 24.2) \text{ cm}^3$$

# Question 1: Propagation of Error I (Sphere Volume)

## Problem Statement
The radius of a sphere is measured to be:
$$r = (6.20 \pm 0.05) \text{ cm}$$

Calculate the volume of the sphere ($V$) and its associated absolute uncertainty ($\delta V$).

---

## Step-by-Step Solution

### Step 1: Identify the Given Variables
From the measurement data, we can separate the nominal (central) value and its absolute uncertainty:
* Nominal radius ($r$) = $6.20 \text{ cm}$
* Absolute uncertainty of the radius ($\delta r$) = $0.05 \text{ cm}$

### Step 2: Recall the Geometric Formula
The formula to calculate the volume ($V$) of a perfect sphere based on its radius ($r$) is:
$$V = \frac{4}{3}\pi r^3$$

### Step 3: Calculate the Nominal Volume ($V$)
Substitute the nominal value of the radius ($r = 6.20 \text{ cm}$) into the geometric formula:
$$V = \frac{4}{3} \cdot \pi \cdot (6.20)^3$$

1. First, calculate the cube of the radius:
   $$(6.20)^3 = 6.20 \cdot 6.20 \cdot 6.20 = 238.328 \text{ cm}^3$$

2. Multiply by $\pi$ (using $\pi \approx 3.14159265$):
   $$238.328 \cdot 3.14159265 \approx 748.7228 \text{ cm}^3$$

3. Multiply by $\frac{4}{3}$:
   $$V = \frac{4}{3} \cdot 748.7228 \approx 998.3064 \text{ cm}^3$$

### Step 4: Derive the Error Propagation Formula
According to the rules of calculus-based error propagation, when a function involves a variable raised to a power ($z = x^n$), the relative uncertainty is calculated as:
$$\frac{\delta z}{z} = |n| \cdot \frac{\delta x}{x}$$

Since our volume formula is $V = \frac{4}{3}\pi r^3$, the constant multiplier $\frac{4}{3}\pi$ has no uncertainty ($\delta = 0$). Therefore, the power rule applies directly to $r^3$ (where $n = 3$):
$$\frac{\delta V}{V} = 3 \cdot \frac{\delta r}{r}$$

### Step 5: Calculate the Absolute Uncertainty ($\delta V$)
To find the absolute uncertainty $\delta V$, we rearrange the equation from Step 4:
$$\delta V = 3 \cdot \left( \frac{\delta r}{r} \right) \cdot V$$

Now, substitute the known values into this equation:
$$\delta V = 3 \cdot \left( \frac{0.05 \text{ cm}}{6.20 \text{ cm}} \right) \cdot 998.3064 \text{ cm}^3$$

1. Calculate the fractional (relative) uncertainty of the radius:
   $$\frac{0.05}{6.20} \approx 0.0080645$$

2. Multiply by the power of 3:
   $$3 \cdot 0.0080645 = 0.0241935 \quad \text{(This is the 2.42\% relative uncertainty of the volume)}$$

3. Multiply by the nominal volume to get the absolute uncertainty:
   $$\delta V = 0.0241935 \cdot 998.3064 \approx 24.1525 \text{ cm}^3$$

### Step 6: Apply Significant Figures and Rounding Rules
In experimental physics, absolute uncertainties are typically rounded to **one or two significant figures**. Let's round $\delta V$ to one decimal place to preserve precision clarity:
* $\delta V \approx 24.2 \text{ cm}^3$

The nominal value ($V$) must be rounded to match the same decimal position as the uncertainty:
* $V \approx 998.3 \text{ cm}^3$

---

## Final Answer
The final calculated volume with its propagated uncertainty is:
$$V = (998.3 \pm 24.2) \text{ cm}^3$$

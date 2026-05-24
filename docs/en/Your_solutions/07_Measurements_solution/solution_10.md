# Question 10: Quantitative Light Speed Measurement via Standing Microwave Waves

## 1. Objective and Problem Statement
The objective of this experimental analysis is to calculate the local velocity of electromagnetic radiation (light speed, $c$) using a thermal standing wave boundary condition inside a conventional domestic microwave oven. 

By deactivating the rotational turntable mechanism, localized thermal hotspots are induced on a continuous absorbing medium (chocolate). The spatial separation between adjacent erodes (melted points) correlates to nodes and antinodes of the electric field vector.

### Given Experimental Parameters:
* **Measured Spatial Interval between nodes ($d$):** $6.1 \text{ cm} = 0.061 \text{ m}$
* **Operating Magnetron Frequency ($f$):** $2.45 \text{ GHz} = 2.45 \times 10^9 \text{ Hz}$
* **Reference Velocity Constants ($c_{\text{true}}$):** $3.00 \times 10^8 \text{ m/s}$

---

## 2. Theoretical Framework & Wave Mechanics

Inside a microwave cavity, the superposition of a forwarded planar electromagnetic wave and its reflection from the internal metallic walls produces a static spatial configuration known as a **standing wave**. 

The spatial distribution of the electric field intensity forms nodes (zero amplitude) and antinodes (maximum amplitude). Thermal energy deposition occurs primarily at the antinodes. The physical distance between two consecutive antinodes (or adjacent melted points on the chocolate) corresponds to exactly half of a full wavelength ($\lambda/2$).

Therefore, the boundary condition dictates:
$$d = \frac{\lambda}{2} \implies \lambda = 2d$$

Once the true physical wavelength ($\lambda$) is isolated, the wave speed equation can be invoked to determine the velocity of propagation ($c$):
$$c = f \cdot \lambda$$

---

## 3. Step-by-Step Analytical Calculation

### Step 3.1: Metric Optimization & Parameter Extraction
To maintain SI base unit coherence across the numerical pipeline, convert centimeter readings to meters:
* $d = 6.1 \text{ cm} = 6.1 \times 10^{-2} \text{ m} = 0.061 \text{ m}$
* $f = 2.45 \text{ GHz} = 2.45 \times 10^9 \text{ Hz}$

### Step 3.2: Compute the Physical Wavelength ($\lambda$)
Multiply the node-to-node spatial interval by two:
$$\lambda = 2 \cdot d$$
$$\lambda = 2 \cdot 0.061 \text{ m} = 0.122 \text{ m}$$

### Step 3.3: Compute the Velocity of Light ($c$)
Substitute the absolute frequency and calculated wavelength parameters into the wave function:
$$c = f \cdot \lambda$$
$$c = (2.45 \times 10^9 \text{ s}^{-1}) \cdot (0.122 \text{ m})$$
$$c = 298900000 \text{ m/s} = 2.989 \times 10^8 \text{ m/s}$$

### Step 3.4: Compute the Experimental Percentage Error ($\text{E}_{\%}$)
To benchmark the precision of this qualitative setup, evaluate the absolute fractional deviation relative to the established universal speed of light constant ($c_{\text{true}} = 3.00 \times 10^8 \text{ m/s}$). 

*Note: The absolute value bars are written using GitHub-safe `\left|` and `\right|` syntaxes to fix the syntax errors.*

$$\text{E}_{\%} = \frac{\left| c_{\text{true}} - c_{\text{measured}} \right|}{c_{\text{true}}} \times 100\%$$

$$\text{E}_{\%} = \frac{\left| 300000000 - 298900000 \right|}{300000000} \times 100\%$$

$$\text{E}_{\%} = \frac{1100000}{300000000} \times 100\% \approx 0.366667\%$$

Adhering to standard empirical rounding rules to three significant figures:

$$\text{E}_{\%} \approx 0.37\%$$

---

## 4. Final Scientific Metrological Report
The experimental velocity of electromagnetic waves inside the cavity is calculated as:
$$c = 2.99 \times 10^8 \text{ m/s}$$

The quantitative discrepancy between the empirical measurement and the true velocity of light constant is constrained to a percentage error of **$0.37\%$**. This negligible deviation confirms the high metrological validity of using boundary-layer standing wave methods for measuring universal constant baselines.

# Question 6: Metrological Instrument Precision and Absolute Uncertainty

## 1. Objective and Problem Statement
In experimental physics and metrology, every instrument has an inherent limit to its precision. For digital displays, the uncertainty is determined by the resolution of the last visible digit.

A digital thermometer displays a temperature reading of:
$$T = 25.4^\circ\text{C}$$

Assuming the scientific convention that the absolute uncertainty ($\delta T$) is equal to **half the value of the last visible digit**, determine the exact absolute uncertainty of this measurement.

---

## 2. Theoretical Framework
Unlike analog scales (where observers estimate between lines), digital instruments automatically round the true physical value to the nearest stable digit. 

When a digital screen displays $25.4^\circ\text{C}$, it implies that the true underlying temperature lies somewhere within the rounding boundary of that last decimal place. The resolution ($R$) of an instrument is the smallest incremental change it can detect or display. 

The standard convention for a stable digital readout states:
$$\text{Absolute Uncertainty } (\delta) = \frac{\text{Resolution } (R)}{2}$$

---

## 3. Step-by-Step Analytical Solution

### Step 3.1: Determine the Instrument Resolution ($R$)
Look at the given reading: $25.4^\circ\text{C}$.
The last visible digit is in the tenths place ($0.1$). This means the thermometer increments by steps of $0.1^\circ\text{C}$. 
* **Resolution ($R$):** $0.1^\circ\text{C}$

### Step 3.2: Apply the Digital Precision Rule
According to the problem's criteria, we calculate the absolute uncertainty ($\delta T$) by taking half of the instrument's resolution:
$$\delta T = \frac{R}{2}$$

Substitute $R = 0.1^\circ\text{C}$ into the equation:
$$\delta T = \frac{0.1^\circ\text{C}}{2}$$

Executing the division yields:
$$\delta T = 0.05^\circ\text{C}$$

### Step 3.3: Understand the Physical Meaning
This absolute uncertainty means the true temperature $T_{\text{true}}$ is bounded by the interval:
$$25.4^\circ\text{C} - 0.05^\circ\text{C} \le T_{\text{true}} < 25.4^\circ\text{C} + 0.05^\circ\text{C}$$
$$25.35^\circ\text{C} \le T_{\text{true}} < 25.45^\circ\text{C}$$

Any actual temperature within this range is automatically rounded by the digital hardware to $25.4^\circ\text{C}$.

---

## 4. Final Scientific Conclusion
The absolute uncertainty of the digital thermometer measurement is **$\pm 0.05^\circ\text{C}$**. 

Expressed in standard experimental nomenclature, the complete measurement statement is:
$$T = (25.40 \pm 0.05)^\circ\text{C}$$

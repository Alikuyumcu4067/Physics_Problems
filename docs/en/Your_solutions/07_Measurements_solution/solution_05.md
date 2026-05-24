# Question 5: Determination of Fractional and Percentage Uncertainty

## 1. Objective and Problem Statement
In experimental physics, quantifying the relative scale of an error in comparison to the magnitude of the measured quantity is essential for assessing data quality. 

A temporal measurement is recorded with its absolute uncertainty as follows:
$$t = (5.45 \pm 0.22) \text{ seconds}$$

The objective is to calculate the precise **percentage uncertainty** ($\text{U}_{\%}$) of this measurement.

---

## 2. Theoretical Framework
While absolute uncertainty ($\delta t$) defines the raw margin of error in the same units as the measurand, it does not inherently reflect the precision of the experiment. To standardize this, we define two metrics:

1. **Fractional (Relative) Uncertainty ($\text{U}_{\text{f}}$):** The dimensionless ratio of the absolute uncertainty to the nominal value.
   $$\text{U}_{\text{f}} = \frac{\delta t}{t}$$

2. **Percentage Uncertainty ($\text{U}_{\%}$):** The fractional uncertainty scaled to a percentage framework to define the relative precision.
   $$\text{U}_{\%} = \left( \frac{\delta t}{t} \right) \times 100\%$$

---

## 3. Analytical Treatment & Calculations

### Step 3.1: Parameter Extraction
From the empirical data provided, the core parameters are defined as:
* **Nominal Value of Time ($t$):** $5.45 \text{ s}$
* **Absolute Uncertainty ($\delta t$):** $0.22 \text{ s}$

### Step 3.2: Substitution and Fractional Evaluation
Substituting the extracted parameters into the fractional uncertainty model yields:
$$\text{U}_{\text{f}} = \frac{0.22 \text{ s}}{5.45 \text{ s}} \approx 0.04036697$$

*(Note: The temporal units ($\text{s}$) cancel out, confirming that relative metrics are strictly dimensionless).*

### Step 3.3: Percentage Scaling and Precision Rounding
To convert the dimensionless ratio into percent notation, multiply by $100$:
$$\text{U}_{\%} = 0.04036697 \times 100\% = 4.036697\%$$

Adhering to standard metrological protocols, uncertainty percentages derived from raw absolute data are conventionally restricted to **two or three significant figures** depending on the propagation bounds. Rounding to two decimal places maintains strict consistency with the input parameters:
$$\text{U}_{\%} \approx 4.04\%$$

---

## 4. Final Scientific Conclusion
The percentage uncertainty associated with the temporal measurement $t$ is determined to be **$4.04\%$**. This indicates a high level of experimental precision, as the margin of error accounts for less than $5\%$ of the total measured magnitude.

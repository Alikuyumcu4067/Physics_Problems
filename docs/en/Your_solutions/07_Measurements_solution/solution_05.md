# Question 5: Quantitative Percentage Uncertainty Analysis

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

## 3. Step-by-Step Analytical Calculation

### Step 3.1: Parameter Extraction
From the empirical data provided, we isolate the two key core components:
* **Nominal Value of Time ($t$):** $5.45 \text{ s}$
* **Absolute Uncertainty ($\delta t$):** $0.22 \text{ s}$

### Step 3.2: Calculate the Fractional Uncertainty
Substitute the extracted parameters into the fractional uncertainty equation:
$$\text{U}_{\text{f}} = \frac{0.22 \text{ s}}{5.45 \text{ s}}$$

Executing the division:
$$\text{U}_{\text{f}} \approx 0.040366972$$

*(Note: The temporal units of seconds ($\text{s}$) in the numerator and denominator cancel out completely, confirming that relative metrics are strictly dimensionless).*

### Step 3.3: Calculate the Percentage Uncertainty
To convert the dimensionless fractional ratio into percent notation, multiply the value by $100\%$:
$$\text{U}_{\%} = \text{U}_{\text{f}} \times 100\%$$
$$\text{U}_{\%} = 0.040366972 \times 100\% = 4.0366972\%$$

### Step 3.4: Apply Metrological Rounding Rules
Adhering to standard metrological protocols, final uncertainty percentages derived from raw data are conventionally restricted to **two or three significant figures** depending on the precision of the input apparatus. 

Rounding our result to three significant figures (two decimal places) to maintain mathematical consistency with the original data precision yields:
$$\text{U}_{\%} \approx 4.04\%$$

---

## 4. Final Scientific Conclusion
The percentage uncertainty associated with the temporal measurement $t$ is determined to be **$4.04\%$**. This indicates a high level of experimental precision, as the total experimental margin of error accounts for less than $5\%$ of the measured baseline magnitude.

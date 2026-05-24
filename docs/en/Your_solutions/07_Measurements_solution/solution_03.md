# Question 3: Propagation of Error III (Ohm's Law)

## Problem Statement
The resistance $R$ is calculated using Ohm's Law, $R = \frac{V}{I}$. If the voltage and current are measured as:
$$V = (10.0 \pm 0.2) \text{ V}$$
$$I = (2.00 \pm 0.05) \text{ A}$$

What is the calculated resistance ($R$) and its associated absolute uncertainty ($\delta R$)?

---

## Step-by-Step Solution

### Step 1: Identify the Given Variables
From the problem statement, we extract the nominal (central) values and their respective absolute uncertainties:
* Nominal voltage ($V$) = $10.0 \text{ V}$
* Absolute uncertainty of voltage ($\delta V$) = $0.2 \text{ V}$
* Nominal current ($I$) = $2.00 \text{ A}$
* Absolute uncertainty of current ($\delta I$) = $0.05 \text{ A}$

### Step 2: Recall the Mathematical Formula
According to Ohm's Law, the resistance ($R$) is the quotient of voltage divided by current:
$$R = \frac{V}{I}$$

### Step 3: Calculate the Nominal Resistance ($R$)
Substitute the nominal values of voltage and current into the formula:
$$R = \frac{10.0 \text{ V}}{2.00 \text{ A}} = 5.00 \, \Omega$$

### Step 4: Derive the Error Propagation Formula for Division
Just like multiplication, when a calculated value is the quotient of two independent measurements ($Z = \frac{X}{Y}$), their relative (fractional) uncertainties combine in quadrature (root-sum-of-squares):

$$\frac{\delta R}{R} = \sqrt{\left(\frac{\delta V}{V}\right)^2 + \left(\frac{\delta I}{I}\right)^2}$$

To isolate the absolute uncertainty ($\delta R$), we multiply both sides by the nominal resistance ($R$):
$$\delta R = R \cdot \sqrt{\left(\frac{\delta V}{V}\right)^2 + \left(\frac{\delta I}{I}\right)^2}$$

### Step 5: Calculate the Absolute Uncertainty ($\delta R$)
Substitute our known values into the error propagation equation:

$$\delta R = 5.00 \cdot \sqrt{\left(\frac{0.2}{10.0}\right)^2 + \left(\frac{0.05}{2.00}\right)^2}$$

1. **Calculate the fractional uncertainties:**
   * For voltage: $\frac{0.2}{10.0} = 0.02 \quad \text{(or } 2\% \text{ relative uncertainty)}$
   * For current: $\frac{0.05}{2.00} = 0.025 \quad \text{(or } 2.5\% \text{ relative uncertainty)}$

2. **Square the fractional uncertainties:**
   * $(0.02)^2 = 0.0004$
   * $(0.025)^2 = 0.000625$

3. **Sum the squared values:**
   $$0.0004 + 0.000625 = 0.001025$$

4. **Take the square root of the sum** (this gives the total relative uncertainty of the resistance):
   $$\sqrt{0.001025} \approx 0.0320156 \quad \text{(or } \approx 3.20\% \text{ relative uncertainty)}$$

5. **Multiply by the nominal resistance** to find the absolute uncertainty:
   $$\delta R = 5.00 \cdot 0.0320156 \approx 0.160078 \, \Omega$$

### Step 6: Apply Significant Figures and Rounding Rules
In experimental physics, absolute uncertainties are typically rounded to **one or two significant figures**. 
* Keeping two significant figures gives: $\delta R \approx 0.16 \, \Omega$

The nominal value ($R = 5.00$) already matches the same decimal position (the hundredths place) as our uncertainty, so no further rounding adjustment is needed for the central value:
* $R = 5.00 \, \Omega$

---

## Final Answer
The final calculated resistance with its propagated uncertainty is:
$$R = (5.00 \pm 0.16) \, \Omega$$

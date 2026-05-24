# Question 2: Propagation of Error II (Rectangular Plate Area)

## Problem Statement
The length ($L$) and width ($W$) of a rectangular plate are measured to be:
$$L = (15.3 \pm 0.1) \text{ cm}$$
$$W = (8.4 \pm 0.1) \text{ cm}$$

Calculate the area of the plate ($A$) and its associated absolute uncertainty ($\delta A$).

---

## Step-by-Step Solution

### Step 1: Identify the Given Variables
From the measurement data, we extract the nominal (central) values and their respective absolute uncertainties:
* Nominal length ($L$) = $15.3 \text{ cm}$
* Absolute uncertainty of length ($\delta L$) = $0.1 \text{ cm}$
* Nominal width ($W$) = $8.4 \text{ cm}$
* Absolute uncertainty of width ($\delta W$) = $0.1 \text{ cm}$

### Step 2: Recall the Geometric Formula
The formula to calculate the area ($A$) of a rectangle is the product of its length and width:
$$A = L \cdot W$$

### Step 3: Calculate the Nominal Area ($A$)
Substitute the nominal values of length and width into the area formula:
$$A = 15.3 \text{ cm} \cdot 8.4 \text{ cm}$$
$$A = 128.52 \text{ cm}^2$$

### Step 4: Derive the Error Propagation Formula for Multiplication
When a calculated value is the product of two or more independent measurements ($Z = X \cdot Y$), the uncertainties add in quadrature. This means we use the root-sum-of-squares of their relative (fractional) uncertainties:

$$\frac{\delta A}{A} = \sqrt{\left(\frac{\delta L}{L}\right)^2 + \left(\frac{\delta W}{W}\right)^2}$$

To find the absolute uncertainty ($\delta A$), we multiply both sides by the nominal area ($A$):
$$\delta A = A \cdot \sqrt{\left(\frac{\delta L}{L}\right)^2 + \left(\frac{\delta W}{W}\right)^2}$$

### Step 5: Calculate the Absolute Uncertainty ($\delta A$)
Now, substitute our known values into the error propagation equation:

$$\delta A = 128.52 \cdot \sqrt{\left(\frac{0.1}{15.3}\right)^2 + \left(\frac{0.1}{8.4}\right)^2}$$

1. **Calculate the fractional uncertainties:**
   * For length: $\frac{0.1}{15.3} \approx 0.006536$
   * For width: $\frac{0.1}{8.4} \approx 0.011905$

2. **Square the fractional uncertainties:**
   * $\left(\frac{0.1}{15.3}\right)^2 \approx (0.006536)^2 \approx 0.00004272$
   * $\left(\frac{0.1}{8.4}\right)^2 \approx (0.011905)^2 \approx 0.00014173$

3. **Sum the squared values:**
   $$0.00004272 + 0.00014173 = 0.00018445$$

4. **Take the square root of the sum** (this gives the total relative uncertainty of the area):
   $$\sqrt{0.00018445} \approx 0.013581 \quad \text{(or } 1.36\% \text{ relative uncertainty)}$$

5. **Multiply by the nominal area** to get the absolute uncertainty:
   $$\delta A = 128.52 \cdot 0.013581 \approx 1.7454 \text{ cm}^2$$

### Step 6: Apply Significant Figures and Rounding Rules
In experimental physics, absolute uncertainties are typically rounded to **one or two significant figures**. Let's round $\delta A$ to one decimal place to remain clean and consistent with the original data precision:
* $\delta A \approx 1.7 \text{ cm}^2$

The nominal area ($A$) must be rounded to match the same decimal position as the uncertainty (the tenths place):
* $A \approx 128.5 \text{ cm}^2$

---

## Final Answer
The final calculated area with its propagated uncertainty is:
$$A = (128.5 \pm 1.7) \text{ cm}^2$$

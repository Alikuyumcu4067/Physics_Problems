# Question 6: Metrological Instrument Precision and Absolute Uncertainty

## 1. Problem Statement
A digital thermometer displays a temperature reading of:
$$T = 25.4^\circ\text{C}$$

Assuming the scientific convention that the absolute uncertainty ($\delta T$) is equal to **half the value of the last digit**, calculate the absolute uncertainty of this measurement using a rigorous step-by-step approach.

---

## 2. Step-by-Step Solution

### Step 1: Identify the Component of the Displayed Value
The displayed value is $25.4^\circ\text{C}$. To find the value of the last digit, we look at its decimal position:
* The digit `2` is in the tens place ($2 \times 10$).
* The digit `5` is in the ones place ($5 \times 1$).
* The digit `4` is in the tenths place ($4 \times 0.1$).

The last visible digit resides in the **tenths position**, which means its place value is exactly **$0.1^\circ\text{C}$**.

### Step 2: Determine the Resolution ($R$) of the Instrument
In metrology, the resolution ($R$) is the smallest incremental change that a digital display can physically show. Since this thermometer counts by tenths of a degree, its resolution is:
$$R = 0.1^\circ\text{C}$$

### Step 3: Apply the Core Uncertainty Rule
The problem states the specific scientific constraint for this digital apparatus:
$$\text{Absolute Uncertainty } (\delta T) = \frac{\text{Value of the Last Digit}}{2}$$

Substituting the resolution (value of the last digit) into our constraint formula gives:
$$\delta T = \frac{0.1^\circ\text{C}}{2}$$

### Step 4: Perform the Final Mathematical Division
Now, divide the numerical value to calculate the absolute margin of error:
$$\delta T = 0.1 \div 2 = 0.05^\circ\text{C}$$

### Step 5: Express the Measurement in Standard Metrological Form
When reporting scientific data, the nominal value ($T$) and the absolute uncertainty ($\delta T$) must share the same decimal precision (the same number of digits after the decimal point). 

Since our uncertainty ($0.05^\circ\text{C}$) extends to the hundredths place, we append a trailing zero to our nominal reading ($25.4 \rightarrow 25.40$) to match the precision:
$$T_{\text{final}} = (25.40 \pm 0.05)^\circ\text{C}$$

---

## 3. Physical Interpretation of the Result
An absolute uncertainty of $\pm 0.05^\circ\text{C}$ means that the hardware inside the thermometer rounds any real temperature to the nearest $0.1^\circ\text{C}$. Therefore, the true physical temperature ($T_{\text{true}}$) is mathematically bounded within the following confidence interval:
$$25.35^\circ\text{C} \le T_{\text{true}} < 25.45^\circ\text{C}$$

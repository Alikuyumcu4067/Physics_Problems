# Question 4: Relative Uncertainty (Speedometer)

## Problem Statement
A car's speedometer has a **5% uncertainty**. If the speedometer reads **60 km/h**, what is the range of the car's actual speed?

---

## Step-by-Step Solution

### Step 1: Identify the Given Variables
From the problem description, we can identify the following values:
* Measured Value (Speed, $v$) = $60 \text{ km/h}$
* Relative (Percentage) Uncertainty = $5\% = 0.05$

### Step 2: Understand the Relationship
Relative uncertainty is the ratio of the absolute uncertainty ($\delta v$) to the measured value ($v$). When expressed as a percentage, the formula is:
$$\text{Percentage Uncertainty} = \left( \frac{\delta v}{v} \right) \times 100\%$$

To find the range of the actual speed, we first need to determine the **absolute uncertainty** ($\delta v$), which represents the actual value in km/h that the reading could fluctuate by.

### Step 3: Calculate the Absolute Uncertainty ($\delta v$)
We find the absolute uncertainty by calculating $5\%$ of the measured speed ($60 \text{ km/h}$):
$$\delta v = 60 \text{ km/h} \times 5\%$$
$$\delta v = 60 \times 0.05 = 3 \text{ km/h}$$

This means the speedometer reading is accurate to within $\pm 3 \text{ km/h}$. We can express this measurement as:
$$v = (60 \pm 3) \text{ km/h}$$

### Step 4: Calculate the Lower and Upper Limits of the Range
The "range of actual speed" means finding the minimum and maximum possible speeds the car could realistically be traveling at.

1. **Calculate the Minimum (Lower) Speed Limit:**
   $$v_{\text{min}} = v - \delta v$$
   $$v_{\text{min}} = 60 \text{ km/h} - 3 \text{ km/h} = 57 \text{ km/h}$$

2. **Calculate the Maximum (Upper) Speed Limit:**
   $$v_{\text{max}} = v + \delta v$$
   $$v_{\text{max}} = 60 \text{ km/h} + 3 \text{ km/h} = 63 \text{ km/h}$$

---

## Final Answer
The range of the car's actual speed is between **$57 \text{ km/h}$ and $63 \text{ km/h}$** (inclusive).

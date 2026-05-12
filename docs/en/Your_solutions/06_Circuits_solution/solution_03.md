## 3. Mixed Circuit Analysis

### **Problem Statement**
Calculate the total equivalent resistance ($R_{eq}$) for the complex circuit shown in the figure. 
* **Condition:** All resistors have a value of $R = 5\, \Omega$.

---

### **Step-by-Step Solution**

To solve a mixed circuit, we must simplify it from the "inside out" by identifying the smallest series or parallel combinations.

#### **Step 1: Identify the Right-most Branch**
The two resistors on the far right are connected in **series**.
* **Calculation:** $R_{series\_1} = 5\, \Omega + 5\, \Omega = 10\, \Omega$

#### **Step 2: Parallel Combination (Center-Right)**
The $10\, \Omega$ result from Step 1 is now in **parallel** with the vertical resistor in the middle.
* **Formula:** $\frac{1}{R_p} = \frac{1}{R_1} + \frac{1}{R_2}$
* **Calculation:** $\frac{1}{R_{p\_1}} = \frac{1}{10} + \frac{1}{5} = \frac{1}{10} + \frac{2}{10} = \frac{3}{10}$
* **Result:** $R_{p\_1} = \frac{10}{3} \approx 3.33\, \Omega$

#### **Step 3: Combine with the Horizontal Resistor**
This parallel block ($3.33\, \Omega$) is in **series** with the top horizontal resistor.
* **Calculation:** $R_{series\_2} = 3.33\, \Omega + 5\, \Omega = 8.33\, \Omega$

#### **Step 4: Final Parallel Branch**
The $8.33\, \Omega$ path is in **parallel** with the far-left vertical resistor.
* **Calculation:** $\frac{1}{R_{p\_2}} = \frac{1}{8.33} + \frac{1}{5}$
* **Result:** $R_{p\_2} \approx 3.12\, \Omega$

#### **Step 5: Total Resistance**
Finally, add the remaining resistors on the main input/output lines (if applicable based on the diagram's terminals).
* **Final Calculation:** $R_{total} = R_{p\_2} + R_{bottom} = 3.12 + 5 = \mathbf{8.12\, \Omega}$ *(Note: Final value depends on terminal placement in the image)*

---

### **Final Answer**
The equivalent resistance is approximately **$8.12\, \Omega$**.

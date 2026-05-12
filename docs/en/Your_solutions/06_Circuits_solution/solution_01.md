## 1. Series and Parallel Circuits

### **Problem Statement**
You have three resistors $R_1 = 15\,\Omega$, $R_2 = 30\,\Omega$, and $R_3 = 50\,\Omega$ connected to a **12 V** battery. Calculate the total equivalent resistance ($R_{eq}$) and the total current ($I$) for both configurations.

---

### **Case A: All Connected in Series**

#### **STEP 1: Calculate the Equivalent Resistance ($R_{eq}$)**
In a series circuit, the total resistance is the sum of all individual resistances.
* **Formula:** $R_{eq} = R_1 + R_2 + R_3$
* **Calculation:** $R_{eq} = 15\,\Omega + 30\,\Omega + 50\,\Omega$
* **Result:** **$R_{eq} = 95\,\Omega$**

#### **STEP 2: Calculate the Total Current ($I$)**
Using Ohm's Law, we find the current flowing from the battery.
* **Formula:** $I = \frac{V}{R_{eq}}$
* **Calculation:** $I = \frac{12\,\text{V}}{95\,\Omega}$
* **Result:** **$I \approx 0.126\,\text{A}$**

---

### **Case B: All Connected in Parallel**

#### **STEP 1: Calculate the Equivalent Resistance ($R_{eq}$)**
In a parallel circuit, the reciprocal of the total resistance is the sum of the reciprocals of each resistance.
* **Formula:** $\frac{1}{R_{eq}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3}$
* **Calculation:** $\frac{1}{R_{eq}} = \frac{1}{15} + \frac{1}{30} + \frac{1}{50}$
* **Common Denominator (150):** $\frac{1}{R_{eq}} = \frac{10}{150} + \frac{5}{150} + \frac{3}{150} = \frac{18}{150}$
* **Result:** $R_{eq} = \frac{150}{18} \approx \mathbf{8.33\,\Omega}$

#### **STEP 2: Calculate the Total Current ($I$)**
Using Ohm's Law for the parallel equivalent.
* **Formula:** $I = \frac{V}{R_{eq}}$
* **Calculation:** $I = \frac{12\,\text{V}}{8.33\,\Omega}$
* **Result:** **$I \approx 1.44\,\text{A}$**

---

### **Comparison Table**
| Configuration | Equivalent Resistance ($R_{eq}$) | Battery Current ($I$) |
| :--- | :--- | :--- |
| **Series** | $95\,\Omega$ | $0.126\,\text{A}$ |
| **Parallel** | $8.33\,\Omega$ | $1.44\,\text{A}$ |

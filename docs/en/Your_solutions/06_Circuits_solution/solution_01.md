## 1. Series and Parallel Circuits

### **Problem Statement**
Given a circuit with a **12 V** battery and three resistors:
* $R_1 = 15\, \Omega$
* $R_2 = 30\, \Omega$
* $R_3 = 50\, \Omega$

Calculate the total equivalent resistance ($R_{eq}$) and the current ($I$) flowing from the battery for both **series** and **parallel** configurations.

---

### **Case A: Series Connection**
In a series circuit, the total resistance is the algebraic sum of all individual resistances. The current remains the same through all components.

#### **1. Equivalent Resistance ($R_{eq}$)**
$$R_{eq} = R_1 + R_2 + R_3$$
$$R_{eq} = 15\, \Omega + 30\, \Omega + 50\, \Omega = \mathbf{95\, \Omega}$$

#### **2. Total Current ($I$)**
Using Ohm's Law ($V = I \cdot R$):
$$I = \frac{V}{R_{eq}} = \frac{12\, \text{V}}{95\, \Omega} \approx \mathbf{0.126\, \text{A}}$$

---

### **Case B: Parallel Connection**
In a parallel circuit, the reciprocal of the equivalent resistance is the sum of the reciprocals of each individual resistance. The voltage across each resistor is equal to the battery voltage.

#### **1. Equivalent Resistance ($R_{eq}$)**
$$\frac{1}{R_{eq}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3}$$
$$\frac{1}{R_{eq}} = \frac{1}{15} + \frac{1}{30} + \frac{1}{50}$$

*Finding a common denominator (150):*
$$\frac{1}{R_{eq}} = \frac{10}{150} + \frac{5}{150} + \frac{3}{150} = \frac{18}{150}$$
$$R_{eq} = \frac{150}{18} \approx \mathbf{8.33\, \Omega}$$

#### **2. Total Current ($I$)**
$$I = \frac{V}{R_{eq}} = \frac{12\, \text{V}}{8.33\, \Omega} \approx \mathbf{1.44\, \text{A}}$$

---

### **Results Comparison**

| Configuration | Equivalent Resistance ($R_{eq}$) | Total Current ($I$) |
| :--- | :--- | :--- |
| **Series** | $95\, \Omega$ | $0.126\, \text{A}$ |
| **Parallel** | $8.33\, \Omega$ | $1.44\, \text{A}$ |

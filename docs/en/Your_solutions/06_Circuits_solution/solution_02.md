## 2. Resistors

### **Problem Statement**
You have a supply of exactly three $1\, \Omega$ resistors. What are all the possible equivalent resistances you can create by combining all three of them? List all unique values.

---

### **Possible Combinations**

There are exactly four ways to connect three identical resistors:

#### **1. All in Series**
When all resistors are in a single line, their values add up.
* **Formula:** $R_{eq} = R + R + R$
* **Calculation:** $1 + 1 + 1 = \mathbf{3\, \Omega}$

#### **2. All in Parallel**
When all resistors are connected across the same two nodes.
* **Formula:** $\frac{1}{R_{eq}} = \frac{1}{R} + \frac{1}{R} + \frac{1}{R}$
* **Calculation:** $\frac{1}{R_{eq}} = \frac{1}{1} + \frac{1}{1} + \frac{1}{1} = 3 \Rightarrow R_{eq} = \mathbf{\frac{1}{3} \approx 0.33\, \Omega}$

#### **3. Two in Parallel, One in Series**
Two resistors are branched, and the third one is on the main line.
* **Formula:** $R_{eq} = \left( \frac{R \cdot R}{R + R} \right) + R$
* **Calculation:** $\left( \frac{1 \cdot 1}{1 + 1} \right) + 1 = 0.5 + 1 = \mathbf{1.5\, \Omega}$

#### **4. Two in Series, One in Parallel**
Two resistors are in a line, and the third one is branched across both of them.
* **Formula:** $R_{eq} = \frac{(R + R) \cdot R}{(R + R) + R}$
* **Calculation:** $\frac{(1 + 1) \cdot 1}{(2) + 1} = \frac{2}{3} = \mathbf{\frac{2}{3} \approx 0.67\, \Omega}$

---

### **Summary of Unique Values**
The unique equivalent resistances possible are:
* **$0.33\, \Omega$**
* **$0.67\, \Omega$**
* **$1.5\, \Omega$**
* **$3.0\, \Omega$**

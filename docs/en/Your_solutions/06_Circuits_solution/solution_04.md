## 4. Mixed Circuit Analysis ($10\,\Omega$)

### **Problem Statement**
Calculate the equivalent resistance ($R_{eq}$) for the complex circuit shown in the figure.
* **Condition:** All resistors have a resistance of $R = 10\,\Omega$.

---
To find the total resistance, we simplify the circuit by identifying series and parallel segments, starting from the most "nested" part of the circuit.

#### **Step 1: Simplify the Parallel "Bridge" Section**
Looking at the bottom right of the diagram, there are two resistors connected in **parallel**.
* **Formula:** $R_{p1} = \frac{R \cdot R}{R + R}$
* **Calculation:** $R_{p1} = \frac{10 \cdot 10}{10 + 10} = \frac{100}{20} = \mathbf{5\,\Omega}$

#### **Step 2: Combine Series Resistors (Bottom Branch)**
The $5\,\Omega$ equivalent resistance from Step 1 is in **series** with the resistor immediately to its left.
* **Formula:** $R_{s1} = R + R_{p1}$
* **Calculation:** $R_{s1} = 10 + 5 = \mathbf{15\,\Omega}$

#### **Step 3: Simplify the Top Series Branch**
The two resistors at the top of the circuit are connected in **series**.
* **Formula:** $R_{s2} = R + R$
* **Calculation:** $R_{s2} = 10 + 10 = \mathbf{20\,\Omega}$

#### **Step 4: Combine Parallel Branches**
Now, the top branch ($20\,\Omega$) and the bottom-middle branch ($15\,\Omega$) are in **parallel** with each other.
* **Formula:** $\frac{1}{R_{p2}} = \frac{1}{R_{s1}} + \frac{1}{R_{s2}}$
* **Calculation:** $\frac{1}{R_{p2}} = \frac{1}{15} + \frac{1}{20} = \frac{4+3}{60} = \frac{7}{60}$
* **Result:** $R_{p2} = \frac{60}{7} \approx \mathbf{8.57\,\Omega}$

#### **Step 5: Add the Final Series Resistor**
The entire simplified block ($8.57\,\Omega$) is in **series** with the final resistor on the right before the output terminal.
* **Formula:** $R_{total} = R_{p2} + R$
* **Calculation:** $R_{total} = 8.57 + 10 = \mathbf{18.57\,\Omega}$

---

### **Final Answer**
The total equivalent resistance for the circuit is:
**$$R_{eq} \approx 18.57\,\Omega$$**

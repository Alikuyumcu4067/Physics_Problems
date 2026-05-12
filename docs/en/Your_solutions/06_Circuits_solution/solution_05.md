## 5. Kirchhoff's Laws Analysis

### **Problem Statement**
Find the currents $I_1, I_2, I_3$ flowing through resistors $R_1, R_2, R_3$ respectively in the two-loop circuit.
* **Left Loop:** Ammeter $A$, $R_1 = 20\,\Omega$, $\mathcal{E}_1 = 4.5\,\text{V}$, $r_w = 1\,\Omega$.
* **Right Loop:** $\mathcal{E}_2 = 9\,\text{V}$, $r_w = 1\,\Omega$.
* **Shared Branch:** $R_2 = 10\,\Omega$.

---


**STRETEGY:** We will use Kirchhoff's Junction Rule (Current Law) and Loop Rule (Voltage Law).

#### **STEP 1: Apply Kirchhoff’s Junction Rule**
At the top-right node, the sum of currents entering equals the sum of currents leaving.
* **Equation:** $$I_1 + I_3 = I_2$$

#### **STEP 2: Apply Kirchhoff’s Loop Rule (Left Loop)**
Traversing the left loop clockwise, starting from the bottom-left corner:
* Sum of voltages: $\mathcal{E}_1 - I_1(R_1 + r_w) - I_2(R_2) = 0$
* Substitute values: $4.5 - I_1(20 + 1) - 10I_2 = 0$
* **Equation 1:** $$4.5 - 21I_1 - 10I_2 = 0$$

#### **STEP 3: Apply Kirchhoff’s Loop Rule (Right Loop)**
Traversing the right loop counter-clockwise from the bottom node:
* Sum of voltages: $\mathcal{E}_2 - I_3(r_w) - I_2(R_2) = 0$
* Substitute values: $9 - 1I_3 - 10I_2 = 0$
* **Equation 2:** $$9 - I_3 - 10I_2 = 0$$

#### **STEP 4: Solve the System of Equations**
From the Junction Rule, we know $I_3 = I_2 - I_1$. Substitute this into Equation 2:
1. $9 - (I_2 - I_1) - 10I_2 = 0 \Rightarrow 9 + I_1 - 11I_2 = 0$
2. From Equation 1: $10I_2 = 4.5 - 21I_1 \Rightarrow I_2 = 0.45 - 2.1I_1$

Substitute $I_2$ back into the simplified Equation 2:
* $9 + I_1 - 11(0.45 - 2.1I_1) = 0$
* $9 + I_1 - 4.95 + 23.1I_1 = 0$
* $4.05 + 24.1I_1 = 0 \Rightarrow I_1 \approx -0.168\,\text{A}$ (Negative sign means current flows opposite to the assumed direction).

#### **STEP 5: Calculate Remaining Currents**
* **$I_2$ Calculation:** $I_2 = 0.45 - 2.1(-0.168) \approx \mathbf{0.803\,\text{A}}$
* **$I_3$ Calculation:** $I_3 = I_2 - I_1 = 0.803 - (-0.168) \approx \mathbf{0.971\,\text{A}}$

---

### **Final Results**
* **Current $I_1$ (Left Loop):** $-0.168\,\text{A}$
* **Current $I_2$ (Shared Branch):** $0.803\,\text{A}$
* **Current $I_3$ (Right Loop):** $0.971\,\text{A}$

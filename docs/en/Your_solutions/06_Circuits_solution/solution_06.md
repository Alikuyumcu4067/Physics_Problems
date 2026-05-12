## 6. Kirchhoff's Laws Again

### **Problem Statement**
Calculate the current flowing through the ammeter ($A$) in the multi-loop circuit shown in the diagram.
* **Top Loop:** $\mathcal{E}_2 = 4.5\,\text{V}$, $r_w = 1\,\Omega$, $R_2 = 20\,\Omega$.
* **Bottom Loop:** $\mathcal{E}_1 = 9\,\text{V}$, $r_w = 1\,\Omega$, $R_1 = 10\,\Omega$.

---



#### **STEP 1: Define Current Directions**
Let’s assume the current from the bottom source $\mathcal{E}_1$ is $I_1$ (flowing clockwise) and the current from the top source $\mathcal{E}_2$ is $I_2$ (flowing counter-clockwise). The ammeter is positioned such that it measures the sum or difference of these currents depending on the junction.

#### **STEP 2: Apply Loop Rule to the Top Loop**
Starting from the node before the ammeter and moving clockwise through the top branch:
* **Equation:** $\mathcal{E}_2 - I_2(r_w) - I_2(R_2) = 0$
* **Substitution:** $4.5 - I_2(1) - I_2(20) = 0$
* **Result:** $4.5 - 21I_2 = 0 \Rightarrow I_2 = \frac{4.5}{21} \approx \mathbf{0.214\,\text{A}}$

#### **STEP 3: Apply Loop Rule to the Bottom Loop**
Moving clockwise through the bottom branch:
* **Equation:** $\mathcal{E}_1 - I_1(r_w) - I_1(R_1) = 0$
* **Substitution:** $9 - I_1(1) - I_1(10) = 0$
* **Result:** $9 - 11I_1 = 0 \Rightarrow I_1 = \frac{9}{11} \approx \mathbf{0.818\,\text{A}}$

#### **STEP 4: Calculate Ammeter Reading**
The ammeter ($A$) is located at the junction where these loops meet. Based on the circuit topology, it measures the total current entering the shared branch.
* **Calculation:** $I_{total} = I_1 + I_2$
* **Substitution:** $I_{total} = 0.818 + 0.214 = \mathbf{1.032\,\text{A}}$

---

### **Final Answer**
The current flowing through the ammeter is:
**$$I_A \approx 1.032\,\text{A}$$**

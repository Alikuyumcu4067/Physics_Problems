## 2. Voltage Divider in Series Circuit

### **Problem Statement**
Two resistors, $R_1 = 100\,\Omega$ and $R_2 = 200\,\Omega$, are connected in series to a **24 V** power supply. 
* Calculate the voltage drop across each resistor ($V_1$ and $V_2$).
* Verify the results using Kirchhoff's Voltage Law (KVL).

---



#### **STEP 1: Calculate Total Resistance ($R_{eq}$)**
Since the resistors are in series, we simply add them together.
* **Formula:** $R_{eq} = R_1 + R_2$
* **Calculation:** $100\,\Omega + 200\,\Omega = \mathbf{300\,\Omega}$

#### **STEP 2: Calculate Circuit Current ($I$)**
Using Ohm’s Law for the entire circuit to find the common current.
* **Formula:** $I = \frac{V_{total}}{R_{eq}}$
* **Calculation:** $I = \frac{24\,\text{V}}{300\,\Omega} = \mathbf{0.08\,\text{A}}$ (or $80\,\text{mA}$)

#### **STEP 3: Calculate Individual Voltage Drops**
Now, apply Ohm’s Law ($V = I \times R$) to each resistor individually.
* **For $R_1$:** $V_1 = 0.08\,\text{A} \times 100\,\Omega = \mathbf{8\,\text{V}}$
* **For $R_2$:** $V_2 = 0.08\,\text{A} \times 200\,\Omega = \mathbf{16\,\text{V}}$

#### **STEP 4: Verification using KVL**
According to Kirchhoff's Voltage Law, the sum of voltage drops must equal the source voltage.
* **Verification:** $V_{total} = V_1 + V_2$
* **Check:** $8\,\text{V} + 16\,\text{V} = 24\,\text{V}$
* **Status:** **Verified** ✅

---

### **Final Results**
| Component | Resistance | Voltage Drop |
| :--- | :--- | :--- |
| **Resistor 1** | $100\,\Omega$ | $8\,\text{V}$ |
| **Resistor 2** | $200\,\Omega$ | $16\,\text{V}$ |
| **Total** | **$300\,\Omega$** | **$24\,\text{V}$** |

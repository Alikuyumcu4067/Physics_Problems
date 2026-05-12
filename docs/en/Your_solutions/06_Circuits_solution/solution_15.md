## 14. RLC Circuit & Mechanical Analogy

### **Problem Statement**
* Write down the differential equation for a series RLC circuit (Resistor $R$, Inductor $L$, Capacitor $C$) with a voltage source $V(t)$.
* Compare this to the equation of a **damped harmonic oscillator**.
* Identify the analogies between the terms in the two equations.

---



#### **STEP 1: Derive the RLC Circuit Equation**
Using Kirchhoff’s Voltage Law (KVL), the sum of voltages across the inductor, resistor, and capacitor must equal the source voltage:
$$V_L + V_R + V_C = V(t)$$
Substituting the relationships $V_L = L\frac{dI}{dt}$, $V_R = IR$, and $V_C = \frac{q}{C}$, where $I = \frac{dq}{dt}$:
* **Differential Equation:** $$L \frac{d^2q}{dt^2} + R \frac{dq}{dt} + \frac{1}{C}q = V(t)$$

#### **STEP 2: Recall the Damped Harmonic Oscillator Equation**
In mechanics, Newton’s second law for a mass ($m$) on a spring ($k$) with damping ($b$) and an external force ($F$) is:
* **Equation:** $$m \frac{d^2x}{dt^2} + b \frac{dx}{dt} + kx = F(t)$$

#### **STEP 3: Establish the Analogies**
By comparing the two equations term-by-term, we can see that electrical components behave exactly like mechanical components:

| Electrical Term (RLC) | Mechanical Term (Oscillator) | Physical Role |
| :--- | :--- | :--- |
| **Inductance ($L$)** | **Mass ($m$)** | Inertia (Resistance to change in motion/current) |
| **Resistance ($R$)** | **Damping Constant ($b$)** | Dissipation (Energy loss via heat/friction) |
| **Reciprocal Capacitance ($1/C$)** | **Spring Constant ($k$)** | Restoring Force (Potential energy storage) |
| **Charge ($q$)** | **Displacement ($x$)** | State of the system |
| **Current ($I$)** | **Velocity ($v$)** | Rate of change of the state |
| **Voltage ($V$)** | **External Force ($F$)** | Driver of the system |

---

### **Conclusion**
The RLC circuit is the electrical equivalent of a mass-spring-damper system. This mathematical symmetry allows engineers to use the same techniques to solve both electrical and mechanical vibration problems.

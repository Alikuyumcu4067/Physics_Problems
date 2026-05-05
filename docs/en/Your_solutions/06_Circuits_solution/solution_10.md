# Electromagnetics & Circuit Analysis

## Case Study 10: Quantitative Analysis of Transient Current in Atmospheric Discharge

### 1. Executive Summary
This report analyzes the electrical characteristics of a lightning strike as a transient event. By evaluating the total charge transfer over a specific temporal window, we derive the **Average Current** ($I_{avg}$), providing insight into the magnitude of atmospheric electrical phenomena.

---

### 2. Physical Parameters
The following parameters were captured during the discharge event. For precise calculation, all units are synchronized to the **International System of Units (SI)**.

| Parameter | Symbol | Scalar Value | SI Unit |
| :--- | :---: | :--- | :--- |
| **Total Charge Transferred** | $Q$ | $30$ | Coulombs (C) |
| **Duration of Discharge** | $\Delta t$ | $2.0 \times 10^{-3}$ | Seconds (s) |
| **Calculated Average Current** | $I_{avg}$ | $15,000$ | Amperes (A) |

---

### 3. Theoretical Framework
Electric current is defined as the net rate of flow of electric charge through a cross-sectional area. In cases of non-steady flow (transient pulses), the average current is calculated as the ratio of the total charge ($\Delta Q$) to the total time interval ($\Delta t$):



$$I_{avg} = \frac{\Delta Q}{\Delta t}$$

---

### 4. Step-by-Step Analytical Solution

#### Step 4.1: Temporal Unit Conversion
The observed time is given in milliseconds ($ms$). To align with SI standards for Amperage ($Coulombs/Second$):
$$2\text{ ms} = \frac{2}{1000}\text{ s} = 0.002\text{ s}$$

#### Step 4.2: Applying the Current Operator
Integrating the values into our primary equation:
$$I_{avg} = \frac{30\text{ C}}{0.002\text{ s}}$$

#### Step 4.3: Final Computation
$$I_{avg} = 15,000\text{ A}$$

---

### 5. Engineering Significance & Conversion
In power systems and atmospheric physics, values of this magnitude are typically expressed using **Engineering Notation** to improve readability:

*   **Standard Form:** $15,000\text{ A}$
*   **Kiloampere Form:** $15\text{ kA}$
*   **Scientific Notation:** $1.5 \times 10^{4}\text{ A}$

### 6. Conclusion
The analysis concludes that the lightning bolt generates an average current of **$15\text{ kA}$**. While the duration is extremely brief, the current magnitude is sufficient to cause significant thermal expansion and electromagnetic interference (EMI).

---
*Document Ref: ELEC-6-SEC-10 | Author: Gemini AI*

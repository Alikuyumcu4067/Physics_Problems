## 9. Aristarchus’ Method (Geometric Analysis)

### Step 1: Compute Earth–Sun Distance ($d_{ES}$)
Using the right-triangle configuration during the lunar dichotomy:
$$d_{ES} = \frac{d_{EM}}{\cos(\theta)}$$

Substituting standard parameters ($d_{EM} = 3.84 \times 10^5 \text{ km}$, $\theta = 89.85^\circ$):
$$d_{ES} = \frac{3.84 \times 10^5 \text{ km}}{\cos(89.85^\circ)} \approx \frac{384,000}{0.002618} \approx 1.467 \times 10^8 \text{ km}$$

### Step 2: Compute Sun's True Diameter ($D_S$)
Convert apparent diameter ($\alpha$) to radians and apply small-angle approximation:
$$\alpha = 0.53^\circ \times \frac{\pi}{180^\circ} \approx 0.00925 \text{ rad}$$
$$D_S \approx \alpha \times d_{ES} = 0.00925 \times 1.467 \times 10^8 \text{ km} \approx 1.357 \times 10^6 \text{ km}$$

### Step 3: Determine Diameter Ratio ($D_M / D_S$)
Since both bodies exhibit identical angular constraints ($\alpha$):
$$\frac{D_M}{D_S} = \frac{d_{EM}}{d_{ES}} = \cos(89.85^\circ) \approx 0.00262 \quad \left(\frac{1}{382}\right)$$

### Step 4: Sensitivity Evaluation Using Historical $\theta = 89.75^\circ$
$$d_{ES,\text{new}} = \frac{3.84 \times 10^5 \text{ km}}{\cos(89.75^\circ)} \approx \frac{384,000}{0.004363} \approx 8.80 \times 10^7 \text{ km}$$
$$\text{Net Discrepancy:} \quad \Delta d_{ES} = 1.467 \times 10^8 - 8.80 \times 10^7 = 5.87 \times 10^7 \text{ km}$$

---

> **Methodological Comment:** A marginal variance of $0.10^\circ$ induces a roughly $40\%$ change in the output metric. This extreme mathematical sensitivity proves that while Aristarchus' logic was flawless, the framework was highly vulnerable to instrumentation limitations, as pinpointing the precise moment of a half-moon phase cannot be achieved reliably with the naked eye.

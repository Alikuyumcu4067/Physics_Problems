# Section 4: Electromagnetism I - Problem 6

## 6. Electric Field from a System of Point Charges

**Problem:** Two point charges are given: $+q$ at point $(-a, 0)$ and $+2q$ at point $(a, 0)$. 
1. Determine the field vectors $\vec{E}(0, y)$, $\vec{E}(x, 0)$, and the general field $\vec{E}(x, y)$.
2. Determine the conditions for which $E_x = 0, E_y = 0$, and the zero field point $\vec{E} = 0$.
3. Calculate the field for $a = 0.2 \text{ m}, y = 0.3 \text{ m}, q = 2 \mu\text{C}$ at $(0, y)$.
4. Investigate the limit $y \gg a$.

---

### I. General Field Vector $\vec{E}(x, y)$
Using the Principle of Superposition, the total field is the sum of the fields from $q_1$ and $q_2$.
The position vectors for the charges are $\vec{r}_1 = -a\hat{i}$ and $\vec{r}_2 = a\hat{i}$. 
For a general point $P(x, y)$, the displacement vectors are:
* $\vec{r}_{p1} = (x+a)\hat{i} + y\hat{j}$ with magnitude $r_1 = \sqrt{(x+a)^2 + y^2}$
* $\vec{r}_{p2} = (x-a)\hat{i} + y\hat{j}$ with magnitude $r_2 = \sqrt{(x-a)^2 + y^2}$

The general electric field vector is:
$$\vec{E}(x, y) = \frac{kq}{r_1^3} \vec{r}_{p1} + \frac{k(2q)}{r_2^3} \vec{r}_{p2}$$
$$\vec{E}(x, y) = kq \left[ \frac{(x+a)\hat{i} + y\hat{j}}{((x+a)^2 + y^2)^{3/2}} + \frac{2((x-a)\hat{i} + y\hat{j})}{((x-a)^2 + y^2)^{3/2}} \right]$$

---

### II. Specific Field Vectors
**1. Field on the y-axis, $\vec{E}(0, y)$:**
Substitute $x = 0$ into the general formula:
$$\vec{E}(0, y) = kq \left[ \frac{a\hat{i} + y\hat{j}}{(a^2 + y^2)^{3/2}} + \frac{2(-a\hat{i} + y\hat{j})}{(a^2 + y^2)^{3/2}} \right] = \frac{kq}{(a^2 + y^2)^{3/2}} [ (a-2a)\hat{i} + (y+2y)\hat{j} ]$$
$$\vec{E}(0, y) = \frac{kq}{(a^2 + y^2)^{3/2}} (-a\hat{i} + 3y\hat{j})$$

**2. Field on the x-axis, $\vec{E}(x, 0)$:**
Substitute $y = 0$ (Note: signs depend on the region relative to charges):
$$\vec{E}(x, 0) = kq \left[ \frac{(x+a)}{|x+a|^3}\hat{i} + \frac{2(x-a)}{|x-a|^3}\hat{i} \right]$$

---

### III. Conditions for Zero Field ($\vec{E} = 0$)
* **$E_y = 0$:** This occurs anywhere on the x-axis ($y=0$) because the charges lie on the x-axis.
* **$E_x = 0$:** On the y-axis, $E_x$ is never zero (except at infinity) because the $+2q$ charge always pushes harder to the left than the $+q$ charge pushes to the right.
* **Total Zero Field ($\vec{E} = 0$):** This must occur on the x-axis between the two charges (where fields oppose).
    $$\frac{kq}{(x+a)^2} = \frac{k(2q)}{(a-x)^2} \implies \frac{1}{(x+a)^2} = \frac{2}{(a-x)^2}$$
    Taking the root: $a-x = \sqrt{2}(x+a) \implies x = a\frac{1-\sqrt{2}}{1+\sqrt{2}} \approx -0.17a$

---

### IV. Numerical Calculation
**Given:** $a=0.2, y=0.3, q=2\times 10^{-6} \text{ C}$. Point is $(0, 0.3)$.
Distance $r = \sqrt{0.2^2 + 0.3^2} = \sqrt{0.04 + 0.09} = \sqrt{0.13} \approx 0.36 \text{ m}$.
Using the $\vec{E}(0, y)$ formula:
$$\vec{E} = \frac{(9\times 10^9)(2\times 10^{-6})}{(0.13)^{3/2}} (-0.2\hat{i} + 0.9\hat{j})$$
$$\vec{E} \approx 3.84 \times 10^5 (-0.2\hat{i} + 0.9\hat{j}) \text{ V/m}$$

---

### V. Limit Investigation ($y \gg a$)
When $y$ is much larger than $a$, $(a^2 + y^2) \approx y^2$:
$$\vec{E}(0, y) \approx \frac{kq}{(y^2)^{3/2}} (-a\hat{i} + 3y\hat{j}) = \frac{kq}{y^3} (-a\hat{i} + 3y\hat{j})$$
Since $3y \gg a$, the $\hat{i}$ component becomes negligible compared to the $\hat{j}$ component:
$$\vec{E} \approx \frac{3kq}{y^2} \hat{j}$$
**Key Insight:** At large distances, the two charges ($q$ and $2q$) merge effectively into a single point charge of $+3q$, and the field follows the $1/r^2$ law.

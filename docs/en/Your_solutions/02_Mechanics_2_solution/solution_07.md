## 7. Dynamics with Friction (Stacked Blocks)

### Problem Statement
A **5 kg** block ($m_1$) is placed on top of a **10 kg** block ($m_2$). 
- A horizontal force of **45 N** is applied to the 10 kg block.
- The 5 kg block is tied to a wall with a string, preventing it from moving.
- The coefficient of kinetic friction ($\mu_k$) between all surfaces (between blocks and between the bottom block and floor) is **0.2**.

Find the acceleration ($a$) of the 10 kg block.
*(Assume $g = 9.81 \, m/s^2$)*

---

### Analytical Solution

To find the acceleration, we must perform a force analysis on the 10 kg block (Block 2).

#### Step 1: Friction between the two blocks ($f_1$)
Since Block 1 is stationary and Block 2 moves under it, there is kinetic friction between them.
- Normal Force ($N_1$): $m_1 \cdot g = 5 \times 9.81 = 49.05 \, N$
- Friction Force ($f_1$): $\mu_k \cdot N_1 = 0.2 \times 49.05 = \mathbf{9.81 \, N}$

#### Step 2: Friction between the bottom block and the floor ($f_2$)
The floor supports the weight of both blocks.
- Total Mass ($M$): $m_1 + m_2 = 5 + 10 = 15 \, kg$
- Normal Force ($N_2$): $M \cdot g = 15 \times 9.81 = 147.15 \, N$
- Friction Force ($f_2$): $\mu_k \cdot N_2 = 0.2 \times 147.15 = \mathbf{29.43 \, N}$

#### Step 3: Calculation of Net Force ($F_{net}$)
The applied force $F$ must overcome both friction forces ($f_1$ acting on the top surface and $f_2$ acting on the bottom surface).
$$F_{net} = F_{applied} - f_1 - f_2$$
$$F_{net} = 45 - 9.81 - 29.43 = \mathbf{5.76 \, N}$$

#### Step 4: Newton's Second Law
The acceleration of the 10 kg block is:
$$a = \frac{F_{net}}{m_2} = \frac{5.76}{10} = \mathbf{0.576 \, m/s^2}$$

**Result:** The acceleration of the 10 kg block is approximately **0.58 m/s²**.

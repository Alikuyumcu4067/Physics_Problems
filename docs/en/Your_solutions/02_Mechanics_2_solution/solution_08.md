## 8. Work of a Variable Force (Conservative Fields)

### Problem Statement
Given a one-dimensional conservative force:
$$F(x) = -kx$$
1. Write down and solve the equation of motion.
2. Calculate the work done during displacement from $0$ to $x_0$.
3. Interpret the result as potential energy.
4. Verify the relationship $F = -\frac{dU}{dx}$.
5. Describe the graphs of $F(x)$ and $U(x)$.

---

### Analytical Solution

#### 1. Equation of Motion
Using Newton's Second Law ($F = ma$):
$$m \frac{d^2x}{dt^2} = -kx \implies \frac{d^2x}{dt^2} + \frac{k}{m}x = 0$$
This is a second-order linear homogeneous differential equation. The solution is:
$$x(t) = A \cos(\omega t + \phi)$$
where $\omega = \sqrt{k/m}$ is the angular frequency.

#### 2. Work Done
Work done by a variable force is the integral of the force over the displacement:
$$W = \int_{0}^{x_0} F(x) \, dx = \int_{0}^{x_0} (-kx) \, dx$$
$$W = \left[ -\frac{1}{2}kx^2 \right]_{0}^{x_0} = \mathbf{-\frac{1}{2}kx_0^2}$$

#### 3. Potential Energy Interpretation
The change in potential energy ($\Delta U$) is defined as the negative of the work done by a conservative force:
$$\Delta U = -W \implies U(x_0) - U(0) = \frac{1}{2}kx_0^2$$
Assuming $U(0) = 0$, the potential energy stored in the system is **$U(x) = \frac{1}{2}kx^2$**.

#### 4. Verification ($F = -dU/dx$)
$$-\frac{d}{dx} \left( \frac{1}{2}kx^2 \right) = -( \frac{1}{2} \cdot k \cdot 2x ) = -kx$$
The result matches the original force $F(x)$, verifying the conservative nature of

# Optimization Problem Solution

## **11. Dynamics with a Time-Dependent Force Solution**

---

## **Problem**

A particle of mass **$m = 3$ kg** moves in a force field $\vec{F}$ that depends on time:
$$\vec{F}(t) = (15t, 3t - 12, -6t^2) \, \text{N}$$

**Initial Conditions (at $t=0$):**
- Position: $\vec{r}_0 = (5, 2, -3) \, \text{m}$
- Velocity: $\vec{v}_0 = (2, 0, 1) \, \text{m/s}$

Find the dependence of **velocity** and **position** on time.

---

# **Step 1: Calculate the Acceleration ($\vec{a}$)**

👉 According to Newton’s Second Law ($\vec{F} = m\vec{a}$), acceleration is force divided by mass.

---

## 🧠 WHY divide by mass first?
- Acceleration is the "bridge" between force and motion.
- Since $m = 3$ kg, we divide each component of the force vector by 3.

---

## The Calculation:
$$\vec{a}(t) = \frac{\vec{F}(t)}{3} = \left( \frac{15t}{3}, \frac{3t-12}{3}, \frac{-6t^2}{3} \right)$$
$$\vec{a}(t) = (5t, t - 4, -2t^2) \, \text{m/s}^2$$

---

# **Step 2: Find the Velocity ($\vec{v}(t)$)**

👉 Velocity is the **integral** of acceleration: $\vec{v}(t) = \int \vec{a}(t) \, dt + \vec{v}_0$.

---

## 🧠 WHY add $\vec{v}_0$ at the end?
- Integration gives us the *change* in velocity. 
- To find the *actual* velocity at any time, we must start from the initial velocity the particle already had at $t=0$.

---

## The Integration:
- $v_x = \int 5t \, dt = \frac{5}{2}t^2 + v_{0x} = 2.5t^2 + 2$
- $v_y = \int (t - 4) \, dt = \frac{1}{2}t^2 - 4t + v_{0y} = 0.5t^2 - 4t + 0$
- $v_z = \int -2t^2 \, dt = -\frac{2}{3}t^3 + v_{0z} = -\frac{2}{3}t^3 + 1$

**Resulting Velocity Vector:**
$$\vec{v}(t) = (2.5t^2 + 2, 0.5t^2 - 4t, -0.67t^3 + 1) \, \text{m/s}$$

---

# **Step 3: Find the Position ($\vec{r}(t)$)**

👉 Position is the **integral** of velocity: $\vec{r}(t) = \int \vec{v}(t) \, dt + \vec{r}_0$.

---

## 🧠 WHY integrate again?
- Velocity tells us how fast the position is changing. 
- By summing up (integrating) all these small changes over time, we find the particle's path in 3D space.

---

## The Integration:
- $x(t) = \int (2.5t^2 + 2) \, dt = \frac{2.5}{3}t^3 + 2t + x_0 = \frac{5}{6}t^3 + 2t + 5$
- $y(t) = \int (0.5t^2 - 4t) \, dt = \frac{0.5}{3}t^3 - 2t^2 + y_0 = \frac{1}{6}t^3 - 2t^2 + 2$
- $z(t) = \int (-\frac{2}{3}t^3 + 1) \, dt = -\frac{2}{12}t^4 + t + z_0 = -\frac{1}{6}t^4 + t - 3$

---

# **Step 4: Final Vector Form**

Combining everything into the final position vector:

$$\vec{r}(t) = \left( \frac{5}{6}t^3 + 2t + 5, \, \frac{1}{6}t^3 - 2t^2 + 2, \, -\frac{1}{6}t^4 + t - 3 \right) \, \text{m}$$

---

## ✅ **FINAL SUMMARY**

- **Acceleration:** Found by scaling the force vector.
- **Velocity:** First integral + Initial velocity constants.
- **Position:** Second integral + Initial position constants.

👉 **Note:** Notice how the $z$-axis motion is dominated by $t^4$ because the force was already $t^2$. The higher the power of time in the force, the more "aggressive" the displacement becomes!

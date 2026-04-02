# Optimization Problem Solution

## **12. Work and Energy with a Constant Force Solution**

---

## **Problem**

A constant force acts on a body of mass **$m = 2$ kg**:
$$\vec{F} = [6, 2] \, \text{N}$$

**Initial Conditions (at $t=0$):**
- Initial Velocity: $\vec{v}_0 = (1, -1) \, \text{m/s}$
- Initial Position: $\vec{r}_0 = (0, 0) \, \text{m}$

**Find:**
1. Determine $\vec{a}(t)$, $\vec{v}(t)$, and $\vec{r}(t)$.
2. Draw the trajectory (conceptually).
3. Calculate the **work done** ($W$) at $t = 3 \, \text{s}$.
4. Verify the **Work-Energy Theorem**.

---

# **Step 1: Determine $\vec{a}(t)$, $\vec{v}(t)$, and $\vec{r}(t)$**

👉 Since the force is **constant**, the acceleration will also be constant.

---

## 🧠 WHY is constant acceleration important?
- Constant acceleration means we can use simple integration or kinematic equations.
- $\vec{a} = \vec{F} / m = (6/2, 2/2) = (3, 1) \, \text{m/s}^2$.

---

## The Integration:
- **Velocity ($\vec{v}$):** $\int \vec{a} \, dt + \vec{v}_0$
  - $v_x = 3t + 1$
  - $v_y = t - 1$
  - $\vec{v}(t) = (3t + 1, t - 1) \, \text{m/s}$

- **Position ($\vec{r}$):** $\int \vec{v} \, dt + \vec{r}_0$
  - $x(t) = 1.5t^2 + t + 0$
  - $y(t) = 0.5t^2 - t + 0$
  - $\vec{r}(t) = (1.5t^2 + t, 0.5t^2 - t) \, \text{m}$

---

# **Step 2: Trajectory of the Motion**

👉 The trajectory is a **parabola** in the $xy$-plane.

---

## 🧠 WHY a parabola?
- Both $x$ and $y$ are quadratic functions of $t$.
- Since the force (and acceleration) is constant and not parallel to the initial velocity, the path must curve like a projectile.



---

# **Step 3: Calculate Work Done at $t = 3 \, \text{s}$**

👉 Work is the dot product of Force and Displacement: $W = \vec{F} \cdot \Delta \vec{r}$.

---

## 🧠 WHY use the dot product?
- Only the part of the force that points in the direction of the displacement does work.

---

## The Calculation:
First, find the position at $t = 3$:
- $x(3) = 1.5(3)^2 + 3 = 13.5 + 3 = 16.5 \, \text{m}$
- $y(3) = 0.5(3)^2 - 3 = 4.5 - 3 = 1.5 \, \text{m}$
- $\Delta \vec{r} = (16.5, 1.5) \, \text{m}$

Now, calculate $W$:
$$W = \vec{F} \cdot \Delta \vec{r} = (6)(16.5) + (2)(1.5)$$
$$W = 99 + 3 = 102 \, \text{J}$$

---

# **Step 4: Verify the Work-Energy Theorem**

👉 The theorem states: **Work Done = Change in Kinetic Energy** ($W = \Delta K$).

---

## 🧠 WHY check this?
- It confirms that all the energy "pushed" into the object by the force has successfully turned into speed.

---

## The Verification:
1. **Initial Kinetic Energy ($K_0$):**
   - $|\vec{v}_0|^2 = 1^2 + (-1)^2 = 2$
   - $K_0 = \frac{1}{2} m v_0^2 = \frac{1}{2} (2)(2) = 2 \, \text{J}$

2. **Final Kinetic Energy ($K_f$) at $t=3$:**
   - $v_x(3) = 3(3) + 1 = 10$
   - $v_y(3) = 3 - 1 = 2$
   - $|\vec{v}_f|^2 = 10^2 + 2^2 = 104$
   - $K_f = \frac{1}{2} m v_f^2 = \frac{1}{2} (2)(104) = 104 \, \text{J}$

3. **Change in Energy ($\Delta K$):**
   - $\Delta K = 104 - 2 = 102 \, \text{J}$

👉 Since **$W = 102 \, \text{J}$** and **$\Delta K = 102 \, \text{J}$**, the theorem is **Verified!** ✅

---

# **🔥 FINAL SUMMARY**
- **Acceleration:** Constant $(3, 1) \, \text{m/s}^2$.
- **Work Done:** $102 \, \text{J}$.
- **Consistency:** The work done matches the speed increase perfectly.

👉 **Motion is predictable, energy is conserved, and physics is awesome!**

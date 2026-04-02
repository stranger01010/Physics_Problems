# Optimization Problem Solution

## **10. Force Field and Power Solution**

---

## **Problem**

In a certain force field, a particle with mass **$m = 0.5$ kg** moves according to these equations:
$$x = 5t^2 - t$$
$$y = 2t^3$$
$$z = -3t + 2$$

Find the time dependence of:
1. **Velocity** ($\vec{v}$)
2. **Momentum** ($\vec{p}$)
3. **Acceleration** ($\vec{a}$)
4. **Force** ($\vec{F}$)
5. **Power** ($P$)

---

# **Step 1: Calculate the Velocity ($\vec{v}$)**

👉 Velocity is the **first derivative** of position with respect to time ($v = \frac{dr}{dt}$).

---

## 🧠 WHY do we take derivatives separately?
- Each coordinate ($x, y, z$) changes independently in 3D space.
- To find the total velocity vector, we must find the rate of change for each axis.

---

## The Calculation:
- $v_x = \frac{dx}{dt} = \frac{d}{dt}(5t^2 - t) = 10t - 1$
- $v_y = \frac{dy}{dt} = \frac{d}{dt}(2t^3) = 6t^2$
- $v_z = \frac{dz}{dt} = \frac{d}{dt}(-3t + 2) = -3$

**Resulting Velocity Vector:**
$$\vec{v}(t) = (10t - 1, 6t^2, -3) \, \text{m/s}$$

---

# **Step 2: Calculate the Momentum ($\vec{p}$)**

👉 Momentum is the product of mass and velocity ($\vec{p} = m\vec{v}$).

---

## 🧠 WHY multiply by mass?
- Momentum represents the "quantity of motion."
- Since $m = 0.5$ kg, we simply scale the velocity vector by half.

---

## The Calculation:
$$\vec{p}(t) = 0.5 \cdot (10t - 1, 6t^2, -3)$$
$$\vec{p}(t) = (5t - 0.5, 3t^2, -1.5) \, \text{kg·m/s}$$

---

# **Step 3: Calculate the Acceleration ($\vec{a}$)**

👉 Acceleration is the **derivative of velocity** ($a = \frac{dv}{dt}$).

---

## The Calculation:
- $a_x = \frac{d}{dt}(10t - 1) = 10$
- $a_y = \frac{d}{dt}(6t^2) = 12t$
- $a_z = \frac{d}{dt}(-3) = 0$

**Resulting Acceleration Vector:**
$$\vec{a}(t) = (10, 12t, 0) \, \text{m/s}^2$$

---

# **Step 4: Calculate the Force ($\vec{F}$)**

👉 According to Newton’s Second Law: $\vec{F} = m\vec{a}$.

---

## 🧠 WHY is the $z$-component zero?
- Since the velocity in the $z$-direction is constant ($-3$ m/s), there is no change in motion on that axis.
- **No change in motion = No net force.**

---

## The Calculation:
$$\vec{F}(t) = 0.5 \cdot (10, 12t, 0)$$
$$\vec{F}(t) = (5, 6t, 0) \, \text{N}$$

---

# **Step 5: Calculate the Power ($P$)**

👉 Power is the rate at which work is done, calculated by the **dot product** of Force and Velocity ($P = \vec{F} \cdot \vec{v}$).

---

## 🧠 WHY use the dot product?
- Only the component of force acting **in the direction of motion** does work.
- The dot product ($F_x v_x + F_y v_y + F_z v_z$) gives us this scalar value.

---

## The Calculation:
$$P(t) = (5)(10t - 1) + (6t)(6t^2) + (0)(-3)$$
$$P(t) = 50t - 5 + 36t^3 + 0$$

**Rearranging by powers of $t$:**
$$P(t) = 36t^3 + 50t - 5 \, \text{W}$$

---

# **🔥 FINAL SUMMARY**

- **Velocity:** $(10t - 1, 6t^2, -3)$
- **Acceleration:** $(10, 12t, 0)$
- **Force:** Constant on X, increasing on Y.
- **Power:** Increases cubicly with time ($t^3$).

👉 **The field is transferring more energy to the particle as time goes on!**

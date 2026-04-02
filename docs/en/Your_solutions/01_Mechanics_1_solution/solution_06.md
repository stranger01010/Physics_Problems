# Optimization Problem Solution

## **Variable Velocity Solution**

---

## **Problem**

An object's velocity is given by the function:
$$v(t) = t^2 + 2t - 5$$

**Initial Conditions (at $t=0$):**
- Position: $x_0 = 4$

**Find:**
1. The **acceleration** ($a$) at $t = 3$.
2. The **position** ($x$) at $t = 3$.

---

# **Step 1: Find the Acceleration ($a$)**

👉 Acceleration is the **first derivative** of velocity with respect to time ($a = \frac{dv}{dt}$).

---

## 🧠 WHY use a derivative?

- Velocity tells us how position changes.
- Acceleration tells us how **velocity** changes. 
- To find the "rate of change" of velocity at a specific moment, we take the derivative.

---

## The Calculation:

Take the derivative of $v(t) = t^2 + 2t - 5$:
$$a(t) = \frac{d}{dt}(t^2 + 2t - 5)$$
$$a(t) = 2t + 2$$

Now, substitute $t = 3$:
$$a(3) = 2(3) + 2$$
$$a(3) = 6 + 2 = 8 \, \text{m/s}^2$$

---

# **Step 2: Find the Position Function ($x(t)$)**

👉 Position is the **integral** of velocity: $x(t) = \int v(t) \, dt + C$.

---

## 🧠 WHY use an integral?

- Velocity is the derivative of position. 
- To "reverse" a derivative and go back to the original position, we must integrate.
- The constant $C$ represents our starting point ($x_0$).

---

## The Integration:

$$\int (t^2 + 2t - 5) \, dt$$
$$x(t) = \frac{1}{3}t^3 + t^2 - 5t + C$$

Use the initial condition $x(0) = 4$ to find $C$:
$$4 = \frac{1}{3}(0)^3 + (0)^2 - 5(0) + C$$
$$C = 4$$

**Final Position Equation:**
$$x(t) = \frac{1}{3}t^3 + t^2 - 5t + 4$$

---

# **Step 3: Calculate Position at $t = 3$**

Now, substitute $t = 3$ into our new position equation:

$$x(3) = \frac{1}{3}(3)^3 + (3)^2 - 5(3) + 4$$

---

## Calculation:

$$x(3) = \frac{1}{3}(27) + 9 - 15 + 4$$
$$x(3) = 9 + 9 - 15 + 4$$
$$x(3) = 18 - 15 + 4$$
$$x(3) = 7 \, \text{m}$$

---

## ✅ RESULT

👉 At $t = 3$:
- **Acceleration:** $8 \, \text{m/s}^2$
- **Position:** $7 \, \text{m}$

---

# **🔥 FINAL SUMMARY**

- To go from Velocity to Acceleration → **Take the Derivative**.
- To go from Velocity to Position → **Take the Integral**.
- Don't forget the **Initial Position ($x_0$)**; it's the "starting line" of your journey!

👉 **Acceleration:** $8 \, \text{m/s}^2$  
👉 **Position:** $7 \, \text{m}$

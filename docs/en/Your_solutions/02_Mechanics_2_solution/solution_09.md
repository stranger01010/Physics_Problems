# Optimization Problem Solution

## **9. Vertical Throw with Drag Solution**

---

## **Problem**

We have the equation of motion for a mass $m$ subject to gravity and a drag force proportional to velocity ($kv$):
$$m\frac{dv}{dt} = -mg - kv$$
**Initial Conditions:** $v(0) = v_0$, $x(0) = 10$.

1. Solve the equation by **analytical methods**.
2. Determine the **maximum height**.
3. Compare with the **case without drag**.
4. Perform a **numerical simulation** (Python).

---

# **Step 1: Solve the Differential Equation (Velocity)**

👉 We need to find $v(t)$. Let's rearrange the original equation:
$$m\frac{dv}{dt} = -(mg + kv)$$

---

## 🧠 WHY rearrange this way?

- We want to separate the variables ($v$ on one side, $t$ on the other).
- This is a **separable differential equation**.
- As the object moves faster, the $kv$ term grows, reducing the net acceleration.

---

## The Integration:

Divide by $(mg + kv)$ and multiply by $dt/m$:
$$\int \frac{dv}{mg + kv} = -\int \frac{1}{m} \, dt$$

Solving the integral:
$$\frac{1}{k} \ln(mg + kv) = -\frac{t}{m} + C$$

Using the initial condition $v(0) = v_0$ to find $C$:
$$C = \frac{1}{k} \ln(mg + kv_0)$$

---

## Final Velocity Equation:

After exponentiating and isolating $v$:
$$v(t) = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m}t} - \frac{mg}{k}$$

---

# **Step 2: Determine the Maximum Height ($H_{max}$)**

👉 At the highest point, the velocity of the object is **exactly zero** ($v = 0$).

---

## 🧠 WHY solve for $t$ first?

- To find the total displacement, we first need to know **when** the object stops rising ($t_{up}$).
- Setting $v(t) = 0$:
$$0 = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m}t_{up}} - \frac{mg}{k}$$

Solving for $t_{up}$:
$$t_{up} = \frac{m}{k} \ln\left( 1 + \frac{kv_0}{mg} \right)$$

---

## Calculating $H_{max}$:

Integrate $v(t)$ from $0$ to $t_{up}$ and add the starting position ($x_0 = 10$):
$$H_{max} = 10 + \int_{0}^{t_{up}} v(t) \, dt$$

$$H_{max} = 10 + \frac{m v_0}{k} - \frac{m^2 g}{k^2} \ln\left( 1 + \frac{kv_0}{mg} \right)$$

---

# **Step 3: Comparison with "No Drag" Case**

| Feature | With Drag ($-kv$) | No Drag ($k=0$) |
| :--- | :--- | :--- |
| **Velocity** | Decays exponentially | Decreases linearly ($v_0 - gt$) |
| **Max Height** | Lower (energy lost to heat) | Higher ($10 + \frac{v_0^2}{2g}$) |
| **Symmetry** | Non-symmetric (falls slower) | Perfectly symmetric |

---

# **Step 4: Numerical Simulation (Python)**

👉 To visualize the effect of drag, we can use the following code:

```python
import numpy as np
import matplotlib.pyplot as plt

# Parameters
m, g, k = 1.0, 9.81, 0.5
v0, x0 = 20.0, 10.0
t = np.linspace(0, 3, 100)

# Velocity with drag
v_t = (v0 + m*g/k) * np.exp(-k/m*t) - m*g/k

plt.plot(t, v_t, label='With Drag (k=0.5)')
plt.axhline(0, color='black', lw=1)
plt.ylabel('Velocity (m/s)')
plt.xlabel('Time (s)')
plt.title('Vertical Throw with Air Resistance')
plt.legend()
plt.show()

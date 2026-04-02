# Optimization Problem Solution

## **Detailed Variable Velocity Analysis**

---

## **Problem Statement**

An object moves along a straight line with a velocity function:
$$v(t) = t^2 + 2t - 5$$

**Given Initial State ($t=0$):**
- Starting Position ($x_0$): **4 meters**

**Goal:**
Find the **acceleration** and **exact position** when the clock hits **$t = 3$ seconds**.

---

# **Step 1: The "Downwards" Step - Finding Acceleration ($a$)**

👉 To find acceleration from velocity, we look at the **slope** of the velocity curve. In calculus, this means taking the **derivative**.



---

## 🧠 WHY take the derivative?

- **Velocity ($v$)** tells you how fast you are going *right now*.
- **Acceleration ($a$)** tells you how your speed is *changing* at this exact moment.
- By calculating $\frac{dv}{dt}$, we find the instantaneous rate of change.

---

## The Math:

1. **Differentiate the function:**
   $$\frac{d}{dt}(t^2) = 2t$$
   $$\frac{d}{dt}(2t) = 2$$
   $$\frac{d}{dt}(-5) = 0$$

2. **Resulting Acceleration Function:**
   $$a(t) = 2t + 2$$

3. **Plug in $t = 3$:**
   $$a(3) = 2(3) + 2 = 8 \, \text{m/s}^2$$

---

# **Step 2: The "Upwards" Step - Finding Position ($x$)**

👉 To find position from velocity, we calculate the **area under the velocity curve**. In calculus, this is the **integral**.



---

## 🧠 WHY use an integral and a constant ($C$)?

- Integration is like "assembling" all the tiny distances traveled over time.
- However, the velocity formula only tells us how much our position **changed**. It doesn't know where we started.
- That’s why we add **$C$ (the constant of integration)**, which represents our starting coordinate ($x=4$).

---

## The Math:

1. **Integrate the velocity function:**
   $$\int (t^2 + 2t - 5) \, dt = \frac{1}{3}t^3 + t^2 - 5t + C$$

2. **Identify $C$ using the starting point:**
   At $t=0$, we are at $x=4$.
   $$4 = \frac{1}{3}(0)^3 + (0)^2 - 5(0) + C \implies C = 4$$

3. **Final Position Equation:**
   $$x(t) = \frac{1}{3}t^3 + t^2 - 5t + 4$$

---

# **Step 3: Calculating the Final Result at $t = 3$**

Now, let's substitute $t = 3$ into our completed position equation:

$$x(3) = \frac{1}{3}(3)^3 + (3)^2 - 5(3) + 4$$

---

## 🔽 Step-by-Step Breakdown:

- **The Cubic Term:** $\frac{1}{3}(27) = 9$
- **The Squared Term:** $3^2 = 9$
- **The Linear Term:** $-5(3) = -15$
- **The Initial Position:** $+4$

**Summing it up:**
$$9 + 9 - 15 + 4 = 7 \, \text{m}$$

---

# **🔥 FINAL CONCEPTUAL SUMMARY**

| Property | Calculation Type | Value at $t=3$ | Physical Meaning |
| :--- | :--- | :--- | :--- |
| **Position ($x$)** | Integral + $x_0$ | **$7$ m** | Where the object is located. |
| **Velocity ($v$)** | Given Function | **$10$ m/s** | How fast it's moving (calculated as $3^2+2(3)-5$). |
| **Acceleration ($a$)** | Derivative | **$8$ m/s²** | How fast the velocity is increasing. |

---

## ✅ FINAL VERDICT
👉 At 3 seconds, the object is at the **7-meter mark** and its velocity is increasing at a rate of **8 m/s²**.

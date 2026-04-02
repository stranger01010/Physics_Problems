# Optimization Problem Solution

## **8. Work of a Variable Force Solution**

---

## **Problem**

Given a one-dimensional force:
$$F(x) = -kx$$

1. Write down the **equation of motion** and solve it.
2. Calculate the **work done** during displacement from $0$ to $x_0$.
3. Interpret the result as **potential energy**.
4. Verify the relationship $F = -\frac{dU}{dx}$.
5. Draw the graph of $F(x)$ and $U(x)$.

---

# **Step 1: Write and Solve the Equation of Motion**

👉 According to Newton’s Second Law ($F = ma$):
$$-kx = m \frac{d^2x}{dt^2}$$

---

## 🧠 WHY is this equation special?

- This is a **second-order differential equation**.
- It describes **Simple Harmonic Motion (SHM)**.
- The acceleration is always proportional to the displacement but in the opposite direction.

---

## The Solution:

The general solution for this motion is:
$$x(t) = A \cos(\omega t + \phi)$$

Where the angular frequency is:
$$\omega = \sqrt{\frac{k}{m}}$$

---

# **Step 2: Calculate the Work Done ($W$)**

Since the force changes with position ($x$), we cannot just multiply $F \cdot d$. We must **integrate**!

---

## 🧠 WHY use an integral?

- The force $F(x)$ is not constant; it gets stronger as $x$ increases.
- Integral sums up all the tiny amounts of work ($dW$) done over each tiny distance ($dx$).

---

## The Calculation:

$$W = \int_{0}^{x_0} F(x) \, dx$$

Substitute $F(x) = -kx$:
$$W = \int_{0}^{x_0} (-kx) \, dx$$

$$W = -k \left[ \frac{1}{2}x^2 \right]_{0}^{x_0}$$

$$W = -\frac{1}{2}kx_0^2$$

---

# **Step 3: Interpret as Potential Energy ($U$)**

👉 The work done **by the conservative force** is equal to the negative change in potential energy:
$$W = -\Delta U$$

---

## 🧠 WHY is it negative?

- If the force does negative work (like here), it means energy is being **stored** in the system.
- Therefore, the potential energy $U(x)$ is:
$$U(x) = \frac{1}{2}kx^2$$

---

# **Step 4: Verify the Relationship $F = -\frac{dU}{dx}$**

Let's check if the derivative of our energy function gives us the force back.

---

## The Verification:

Take the derivative of $U(x) = \frac{1}{2}kx^2$:
$$\frac{dU}{dx} = \frac{d}{dx} \left( \frac{1}{2}kx^2 \right)$$

$$\frac{dU}{dx} = \frac{1}{2}k \cdot (2x) = kx$$

Now apply the negative sign:
$$-\frac{dU}{dx} = -kx$$

👉 This matches our original force $F(x)$! **Verified.** ✅

---

# **Step 5: Visualizing $F(x)$ and $U(x)$**



---

## 🧠 WHY do the graphs look like this?

- **$F(x) = -kx$**: A straight line passing through the origin with a negative slope (Linear).
- **$U(x) = \frac{1}{2}kx^2$**: A parabola opening upwards (Quadratic).

---

# **🔥 FINAL SUMMARY**

- The negative work ($-\frac{1}{2}kx^2$) means the system is storing energy.
- Force is the **negative gradient** (slope) of the potential energy.
- The motion resulting from this force is always **oscillatory**.

👉 **Work Done:** $-\frac{1}{2}kx_0^2$  
👉 **Potential Energy:** $\frac{1}{2}kx^2$

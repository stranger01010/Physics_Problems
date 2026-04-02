# Optimization Problem Solution

## **1. Gravitational Dependence Solution**

---

## **Problem**

A simple pendulum has a period of **4 seconds on Earth**.

1. What would its period be on the Moon (where gravity is \( \frac{1}{6} \) of Earth)?
2. What length is required for a pendulum to have a period of **1 second on Earth**?

---

# **Step 1: Understand the Physics (Where does the formula come from?)**

The period of a simple pendulum is:

$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

---

## 🔍 What does this formula mean?

- \(T\): time for one full swing (period)  
- \(L\): length of the pendulum  
- \(g\): gravitational acceleration  

---

## 🧠 WHY does this formula exist?

- A pendulum experiences a **restoring force** pulling it back to equilibrium  
- For small angles, this motion becomes **simple harmonic motion (SHM)**  
- In SHM, the period always has the form:

\[
T \sim \frac{1}{\sqrt{\text{restoring force strength}}}
\]

👉 In a pendulum, gravity determines the strength of that restoring force  

---

## 🎯 KEY IDEA:

- If \(g\) increases → stronger pull → faster motion → **smaller period**  
- If \(g\) decreases → weaker pull → slower motion → **larger period**

---

# **Step 2: Compare Earth and Moon**

We are given:

$$
g_{moon} = \frac{g_{earth}}{6}
$$

---

## 🧠 WHY do we use a ratio?

Because:
- The same pendulum → \(L\) does NOT change  
- Only \(g\) changes  

👉 So we compare the two cases using a ratio

---

## Write the ratio:

$$
\frac{T_{moon}}{T_{earth}} = \sqrt{\frac{g_{earth}}{g_{moon}}}
$$

---

## Substitute:

$$
= \sqrt{\frac{g}{g/6}}
$$

$$
= \sqrt{6}
$$

---

# **Step 3: Calculate the Moon Period**

$$
T_{moon} = T_{earth} \cdot \sqrt{6}
$$

---

## 🧠 WHY do we multiply?

- The ratio tells us how much bigger the period becomes  
- So we multiply the original period by that factor  

---

## Calculation:

$$
T_{moon} = 4 \cdot \sqrt{6}
$$

$$
\sqrt{6} \approx 2.45
$$

$$
T_{moon} \approx 4 \cdot 2.45
$$

$$
T_{moon} \approx 9.8 \text{ s}
$$

---

## ✅ RESULT (1)

👉 On the Moon, the pendulum swings **more slowly**  
👉 Period ≈ **9.8 seconds**

---

# **Step 4: Find the Required Length for T = 1 s**

Now we reverse the problem:

👉 We know the period and want to find the length

---

## 🧠 WHY rearrange the formula?

Because:
- We are solving for \(L\), not \(T\)  
- So we must isolate \(L\)

---

## Start from:

$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

---

## Step-by-step rearrangement:

Square both sides:

$$
T^2 = 4\pi^2 \frac{L}{g}
$$

Multiply both sides by \(g\):

$$
gT^2 = 4\pi^2 L
$$

Solve for \(L\):

$$
L = \frac{gT^2}{4\pi^2}
$$

---

# **Step 5: Substitute Values**

$$
L = \frac{9.8 \cdot 1^2}{4\pi^2}
$$

---

## Calculation:

$$
4\pi^2 \approx 39.48
$$

$$
L \approx \frac{9.8}{39.48}
$$

$$
L \approx 0.25 \text{ m}
$$

---

## ✅ RESULT (2)

👉 Required length ≈ **0.25 m (25 cm)**

---

# **🔥 FINAL SUMMARY**

- Lower gravity → slower motion → larger period  
- Moon period ≈ **9.8 s**  
- For a 1-second pendulum → length ≈ **25 cm**

# Optimization Problem Solution

## **2. Harmonic Motion Solution**

---

## **Problem**

A 10 kg mass is attached to a spring and oscillates according to:

$$
x(t) = 0.2 \cos(10\pi t)
$$

1. What is the spring constant \(k\)?  
2. What is the total mechanical energy of the system?

---

# **Step 1: Understand the Given Equation**

We are given:

$$
x(t) = 0.2 \cos(10\pi t)
$$

---

## 🔍 What does this equation mean?

This is the standard form of **simple harmonic motion (SHM)**:

$$
x(t) = A \cos(\omega t)
$$

---

## 🧠 WHY is this important?

Because this form directly tells us:

- \(A\): amplitude (maximum displacement)  
- \(\omega\): angular frequency (how fast it oscillates)  

---

## Compare with given equation:

$$
A = 0.2 \text{ m}
$$

$$
\omega = 10\pi
$$

---

# **Step 2: Find the Spring Constant \(k\)**

In a mass-spring system:

$$
\omega = \sqrt{\frac{k}{m}}
$$

---

## 🧠 WHY this formula?

- The spring provides the restoring force: \(F = -kx\)  
- Using Newton’s second law: \(F = ma\)  
- Combining them leads to SHM, where:

\[
\omega^2 = \frac{k}{m}
\]

---

## Solve for \(k\):

$$
k = m\omega^2
$$

---

## Substitute values:

$$
k = 10 \cdot (10\pi)^2
$$

$$
k = 10 \cdot 100\pi^2
$$

$$
k = 1000\pi^2
$$

---

## Numerical value:

$$
k \approx 1000 \cdot 9.87
$$

$$
k \approx 9870 \text{ N/m}
$$

---

## ✅ RESULT (1)

👉 Spring constant:

$$
k \approx 9870 \text{ N/m}
$$

---

# **Step 3: Find the Total Mechanical Energy**

The total energy in SHM is:

$$
E = \frac{1}{2}kA^2
$$

---

## 🧠 WHY this formula?

- In SHM, energy constantly shifts between:
  - kinetic energy (motion)
  - potential energy (spring compression)

- The **maximum energy** occurs when:
  - displacement is maximum (\(x = A\))
  - velocity is zero

👉 At that point, all energy is stored in the spring:

$$
E = \frac{1}{2}kA^2
$$

---

# **Step 4: Substitute Values**

$$
E = \frac{1}{2} \cdot 1000\pi^2 \cdot (0.2)^2
$$

---

## Calculate step by step:

$$
(0.2)^2 = 0.04
$$

$$
E = \frac{1}{2} \cdot 1000\pi^2 \cdot 0.04
$$

$$
E = 20\pi^2
$$

---

## Numerical value:

$$
E \approx 20 \cdot 9.87
$$

$$
E \approx 197 \text{ J}
$$

---

## ✅ RESULT (2)

👉 Total mechanical energy:

$$
E \approx 197 \text{ J}
$$

---

# **🔥 FINAL SUMMARY**

- From the motion equation, we extract \(A\) and \(\omega\)  
- Use \(\omega = \sqrt{k/m}\) to find the spring constant  
- Use \(E = \frac{1}{2}kA^2\) to find total energy  

---

### Final answers:

- Spring constant: **\(k \approx 9870 \, \text{N/m}\)**  
- Total energy: **\(E \approx 197 \, \text{J}\)**

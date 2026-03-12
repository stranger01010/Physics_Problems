# Optimization Problem Solution

## Problem

A rectangle is placed under the curve

$$
y = 3 - x^2
$$

in the **first quadrant**.
The sides of the rectangle are parallel to the axes.

We need to find the **dimensions of the rectangle that give the maximum area**.

---

# Step 1: Understand the Rectangle

The **top-right corner** of the rectangle touches the curve.

So that point can be written as:

$$
(x,y)
$$

Since the point lies on the curve:

$$
y = 3 - x^2
$$

---

# Step 2: Determine the Dimensions

For the rectangle:

Width = distance along the x-axis

$$
\text{Width} = x
$$

Height = distance along the y-axis

$$
\text{Height} = y
$$

But from the curve we know:

$$
y = 3 - x^2
$$

So the height becomes:

$$
\text{Height} = 3 - x^2
$$

---

# Step 3: Write the Area Function

The formula for the area of a rectangle is

$$
A = \text{width} \times \text{height}
$$

Substitute the expressions we found:

$$
A = x(3 - x^2)
$$

Simplify:

$$
A(x) = 3x - x^3
$$

This function tells us **how the area changes depending on x**.

---

# Step 4: Find the Maximum Area

To find the maximum value, we take the **derivative** of the area function.

$$
A'(x) = 3 - 3x^2
$$

Now set the derivative equal to zero:

$$
3 - 3x^2 = 0
$$

Divide by 3:

$$
1 - x^2 = 0
$$

$$
x^2 = 1
$$

Since the rectangle is in the **first quadrant**, we take the positive value:

$$
x = 1
$$

---

# Step 5: Find the Height

Now substitute (x = 1) into the curve equation.

$$
y = 3 - x^2
$$

$$
y = 3 - 1
$$

$$
y = 2
$$

---

# Final Answer

The rectangle with the **maximum area** has:

Width:

$$
1
$$

Height:

$$
2
$$

Maximum area:

$$
A = 1 \times 2 = 2
$$

So the rectangle dimensions are:

**1 × 2**

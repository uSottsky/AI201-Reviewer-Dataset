# Backpropagation Algorithm Derivation

Thus, for neuron $j$ in the **output** layer, $y_{j}(n)=o_{j}(n)$:
# $\delta_{j}(n)=e_{j}(n)\varphi^{\prime}(v_{j}(n))$
# $=a[d_{j}(n)-o_{j}(n)]o_{j}(n)[1-o_{j}(n)]$

For neuron $j$ in the **hidden** layer
# $\delta_{j}(n)=\varphi^{\prime}(v_{j}(n))\sum_{k}\delta_{k}(n)w_{kj}(n)$
# $=a~y_{j}(n)[1-y_{j}(n)]\sum_{k}\delta_{k}(n)w_{kj}(n)$

24/39

# Supplemental: Calculating Deltas with the Logistic Function (Slide 24)

### Part 1: The Output Neuron Delta ($\delta_j$)
For a neuron $j$ in the final output layer, we usually change its output variable from $y_j(n)$ to $o_j(n)$ just to make it explicitly clear that it is an **output** neuron.

**1. The General Rule:**
From Slide 22, the local gradient for an output neuron is its error multiplied by its activation derivative:
$$\delta_j(n) = e_j(n)\varphi^{\prime}(v_j(n))$$

**2. Expand the Error Term:**
We know the error $e_j(n)$ is just the desired target $d_j(n)$ minus the actual output $o_j(n)$.
$$e_j(n) = d_j(n) - o_j(n)$$

**3. Substitute the Logistic Derivative:**
From Slide 23, we know that for a logistic activation function, the derivative is $a \cdot \text{output} \cdot (1 - \text{output})$. For this output neuron, it looks like this:
$$\varphi^{\prime}(v_j(n)) = a \cdot o_j(n) \cdot [1 - o_j(n)]$$

**4. The Final Output Equation:**
Multiply the expanded error term by the substituted derivative to get the final formula shown on Slide 24:
$$\delta_j(n) = a [d_j(n) - o_j(n)] o_j(n) [1 - o_j(n)]$$

---

### Part 2: The Hidden Neuron Delta ($\delta_j$)
For a neuron $j$ buried inside a hidden layer, we stick to using $y_j(n)$ to represent its output.

**1. The General Rule:**
From Slide 22, the local gradient for a hidden neuron requires looking forward and summing the deltas of the next layer ($k$):
$$\delta_j(n) = \varphi^{\prime}(v_j(n)) \sum_{k} \delta_k(n) w_{kj}(n)$$

**2. Substitute the Logistic Derivative:**
Just like we did for the output neuron, we swap out the ugly derivative notation for our clean, simplified logistic trick:
$$\varphi^{\prime}(v_j(n)) = a \cdot y_j(n) \cdot [1 - y_j(n)]$$

**3. The Final Hidden Equation:**
Plug that directly into the front of the summation to get the final formula shown on Slide 24:
$$\delta_j(n) = a \cdot y_j(n) [1 - y_j(n)] \sum_{k} \delta_k(n) w_{kj}(n)$$

---

### Why is this so important?
Look closely at both final equations. **There is no complex calculus left!** There are no `exp()` functions, no fractions, and no limits. 

To find the error gradients to update the network, a computer only needs to do basic arithmetic (subtraction and multiplication) using numbers it already calculated during the forward pass (the neuron's output, the targets, and the weights). This algebraic simplification is what makes training neural networks computationally fast enough to be practical.

---
# **Navigation**
[[L7B-Slide-23|Previous ← Logistic Function Nonlinearity]]
[[AI 201 - Artificial Intelligence/Lecture 7B Backpropagation/L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-25|Next → Hyperbolic Tangent Nonlinearity]]
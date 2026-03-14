#  Hyperbolic Tangent Function Nonlinearity


When the nonlinearity is the hyperbolic tangent function
# $\varphi(v_{j}(n))=a~tanh(bv_{j}(n))$

the derivative is
# $\varphi^{\prime}(v_{j}(n))=ab~sech^{2}(bv_{j}(n))=ab(1-tanh^{2}(bv_{j}(n)))$
# $\varphi^{\prime}(v_{j}(n))=\frac{b}{a}[a-\varphi(v_{j}(n))][a+\varphi(v_{j}(n))]$                  (14)

Thus, for neuron j in the output layer, $y_{j}(n)=o_{j}(n)$:
# $\delta_{j}(n)=e_{j}(n)\varphi^{\prime}(v_{j}(n))$                                                  (15)
# $\delta_{j}(n)=\frac{b}{a}[d_{j}(n)-o_{j}(n)][a-o_{j}(n)][a+o_{j}(n)]$

For neuron j in the hidden layer
# $\delta_{j}(n)=\varphi^{\prime}(v_{j}(n))\sum_{k}\delta_{k}(n)w_{kj}(n)$                               (16)
# $\delta_{j}(n)=\frac{b}{a}[a-y_{j}(n)][a+y_{j}(n)]\sum_{k}\delta_{k}(n)w_{kj}(n)$


25/39

# Supplemental: Calculating Deltas with the Tanh Function (Slide 25)



### Part 1: Deriving the Tanh Algebraic Trick
First, we need to find the derivative of the scaled Tanh function and simplify it so that it only relies on the neuron's output. 

**1. The Equation:**
The activation function has two scaling parameters, $a$ and $b$:
$$\varphi(v_j(n)) = a \tanh(bv_j(n))$$

**2. The Standard Calculus Derivative:**
Using the chain rule, the derivative of $\tanh(x)$ is $\text{sech}^2(x)$. Because $\text{sech}^2(x)$ is a known trigonometric identity equal to $1 - \tanh^2(x)$, we can write the derivative like this:
$$\varphi^{\prime}(v_j(n)) = ab (1 - \tanh^2(bv_j(n)))$$

**3. The Algebraic Trick:**
We want to get rid of the expensive $\tanh$ operation. From our original equation, we know that $\tanh(bv_j(n)) = \frac{\varphi(v_j(n))}{a}$. Let's substitute that into our derivative:
$$\varphi^{\prime}(v_j(n)) = ab \left( 1 - \left[ \frac{\varphi(v_j(n))}{a} \right]^2 \right)$$

Square the fraction:
$$\varphi^{\prime}(v_j(n)) = ab \left( 1 - \frac{\varphi(v_j(n))^2}{a^2} \right)$$

Find a common denominator ($a^2$) inside the parentheses:
$$\varphi^{\prime}(v_j(n)) = ab \left( \frac{a^2 - \varphi(v_j(n))^2}{a^2} \right)$$

Cancel the $a$ on the outside with one of the $a$'s on the bottom:
$$\varphi^{\prime}(v_j(n)) = \frac{b}{a} \left( a^2 - \varphi(v_j(n))^2 \right)$$

Finally, use the "difference of squares" rule ($x^2 - y^2 = (x-y)(x+y)$) to split it apart:
$$\varphi^{\prime}(v_j(n)) = \frac{b}{a} [a - \varphi(v_j(n))] [a + \varphi(v_j(n))]$$

---

### Part 2: The Output Neuron Delta ($\delta_j$)
For a neuron $j$ in the output layer, its output is denoted as $o_j(n)$. 

**1. The General Rule:**
The local gradient for an output neuron is its error multiplied by its activation derivative:
$$\delta_j(n) = e_j(n) \varphi^{\prime}(v_j(n))$$

**2. Expand the Error Term:**
$$e_j(n) = d_j(n) - o_j(n)$$

**3. Substitute the Tanh Derivative:**
Using our simplified trick from Part 1 (and swapping $\varphi(v_j(n))$ for $o_j(n)$):
$$\varphi^{\prime}(v_j(n)) = \frac{b}{a} [a - o_j(n)] [a + o_j(n)]$$

**4. The Final Output Equation:**
Multiply the error term by the substituted derivative to get Equation 15 from the slide:
$$\delta_j(n) = \frac{b}{a} [d_j(n) - o_j(n)] [a - o_j(n)] [a + o_j(n)]$$

---

### Part 3: The Hidden Neuron Delta ($\delta_j$)
For a neuron $j$ in a hidden layer, its output is denoted as $y_j(n)$.

**1. The General Rule:**
The local gradient for a hidden neuron requires looking forward and summing the deltas of the next layer ($k$):
$$\delta_j(n) = \varphi^{\prime}(v_j(n)) \sum_{k} \delta_k(n) w_{kj}(n)$$

**2. Substitute the Tanh Derivative:**
Swap our simplified trick from Part 1 into the equation (using $y_j(n)$ for the output):
$$\varphi^{\prime}(v_j(n)) = \frac{b}{a} [a - y_j(n)] [a + y_j(n)]$$

**3. The Final Hidden Equation:**
Plug that directly into the front of the summation to get Equation 16 from the slide:
$$\delta_j(n) = \frac{b}{a} [a - y_j(n)] [a + y_j(n)] \sum_{k} \delta_k(n) w_{kj}(n)$$

### Why this matters:
Just like with the logistic function, we've successfully removed all complex calculus from the backpropagation update step. The computer only needs to use addition, subtraction, and multiplication on the outputs it already calculated during the forward pass.

---
# **Navigation**
[[L7B-Slide-24|Previous ← Local Gradient (Logistic)]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-26|Next → The Momentum Term]]
# Backpropagation Algorithm Derivation

Thus
# $\frac{\partial\mathcal{E}(n)}{\partial y_{j}(n)}=\sum_{k}e_{k}(n)\frac{\partial e_{k}(n)}{\partial v_{k}(n)}\frac{\partial v_{k}(n)}{\partial y_{j}(n)}$
# $=-\sum_{k}e_{k}(n)\varphi^{\prime}(v_{k}(n))w_{kj}(n)$
# $=-\sum_{k}\delta_{k}(n)w_{kj}(n)$

and
# $\delta_{j}(n)=-\frac{\partial\mathcal{E}(n)}{\partial y_{j}(n)}\varphi^{\prime}(v_{j}(n))$
# $\delta_{j}(n)=\varphi^{\prime}(v_{j}(n))\sum_{k}\delta_{k}(n)w_{kj}(n)$                                      (12)


21/39


# Supplemental: Deriving the Hidden Neuron Delta (Slide 21)

Slide 21 puts together the final equation for how a hidden neuron $j$ updates its weights. Because a hidden neuron doesn't have a specific target output, its error must be calculated by looking backward at the errors of all the neurons ($k$) it connects to in the next layer.

Here is the step-by-step breakdown of how the equations on this slide are formed, including why the summation is required.

### Step 1: The Core Question - Why is there a Summation ($\sum$)?
In a Multilayer Perceptron, a single hidden neuron $j$ does not just connect to one place; its output signal $y_j$ "fans out" and acts as an input to *multiple* neurons (indexed by $k$) in the next layer. 

Because $y_j$ influences the internal activity ($v_k$) of *every* neuron it connects to, a tiny change in $y_j$ will cause a ripple effect across all those $k$ neurons, ultimately affecting the total network error $\mathcal{E}$.

According to the **multivariate chain rule** in calculus, if a variable ($y_j$) affects a function ($\mathcal{E}$) through multiple distinct intermediate paths ($v_k$), you must calculate the derivative along each individual path and **sum** them all together. 

This is why the derivation for a hidden neuron's error gradient must include $\sum_{k}$: it mathematically gathers up all the separate error ripples caused by neuron $j$.

### Step 2: Assemble the Chain Rule for the Total Error
From Slide 20, using the multivariate chain rule principle explained above, we write the equation for how the total network error ($\mathcal{E}$) changes when the hidden neuron's output ($y_j$) changes:
# $$\frac{\partial\mathcal{E}(n)}{\partial y_{j}(n)} = \sum_{k} e_{k}(n) \frac{\partial e_{k}(n)}{\partial v_{k}(n)} \frac{\partial v_{k}(n)}{\partial y_{j}(n)}$$

### Step 3: Substitute the Solved Partial Derivatives
Also from Slide 20, we already solved the two partial derivatives on the far right:
# 1. $\frac{\partial e_{k}(n)}{\partial v_{k}(n)} = -\varphi^{\prime}(v_{k}(n))$
# 2. $\frac{\partial v_{k}(n)}{\partial y_{j}(n)} = w_{kj}(n)$

Substitute these two results back into the summation:
# $$\frac{\partial\mathcal{E}(n)}{\partial y_{j}(n)} = \sum_{k} e_{k}(n) \Big[ -\varphi^{\prime}(v_{k}(n)) \Big] \Big[ w_{kj}(n) \Big]$$

Pull the negative sign to the front of the summation to get the second line on Slide 21:
# $$\frac{\partial\mathcal{E}(n)}{\partial y_{j}(n)} = -\sum_{k} e_{k}(n) \varphi^{\prime}(v_{k}(n)) w_{kj}(n)$$

### Step 4: Recognize the Local Gradient of the Output Neuron ($\delta_k$)
Look closely at the term $e_{k}(n) \varphi^{\prime}(v_{k}(n))$ inside the summation. 
From Slide 18, we know this exact expression is the definition of the local gradient (the "delta") for the output neuron $k$:
# $$\delta_k(n) = e_k(n) \varphi^{\prime}(v_k(n))$$

By substituting $\delta_k(n)$ into our equation, we vastly simplify it to get the third line on Slide 21:
# $$\frac{\partial\mathcal{E}(n)}{\partial y_{j}(n)} = -\sum_{k} \delta_{k}(n) w_{kj}(n)$$

*Conceptually, this means: The error slope at the hidden neuron's output is simply the sum of the deltas of the next layer's neurons, weighted by the connections between them.*

### Step 5: Calculate the Hidden Neuron's Own Delta ($\delta_j$)
Now we need to find the local gradient for our hidden neuron $j$, which is denoted as $\delta_j(n)$.
From Slide 19, the definition of the local gradient for a hidden neuron is:
# $$\delta_{j}(n) = -\frac{\partial\mathcal{E}(n)}{\partial y_{j}(n)} \varphi^{\prime}(v_{j}(n))$$

### Step 6: The Final Substitution
Take the highly simplified result from Step 4 and plug it into the $\frac{\partial\mathcal{E}(n)}{\partial y_{j}(n)}$ part of the equation in Step 5:
# $$\delta_{j}(n) = - \Bigg[ -\sum_{k} \delta_{k}(n) w_{kj}(n) \Bigg] \varphi^{\prime}(v_{j}(n))$$

The two negative signs cancel each other out ($- \times - = +$). Rearranging the terms slightly to match the slide yields the final equation (Equation 12):
# $$\delta_{j}(n) = \varphi^{\prime}(v_{j}(n)) \sum_{k} \delta_{k}(n) w_{kj}(n)$$

### Conclusion
This final equation is the heart of **Backpropagation**. It proves mathematically that you can calculate the error gradient ($\delta_j$) of any hidden neuron by taking the error gradients of the next layer ($\delta_k$), multiplying them by the weights connecting the layers ($w_{kj}$), **summing them up** (because the signal split into multiple paths), and scaling the result by the derivative of the hidden neuron's own activation function ($\varphi^{\prime}(v_{j}(n))$).



---

# **Navigation**
[[L7B-Slide-20|Previous ← Hidden Neuron Error Gradient]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-22|Next → The Generalized Delta Rule]]
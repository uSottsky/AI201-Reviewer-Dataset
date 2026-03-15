# Backpropagation Algorithm Derivation


# $$\frac{\partial\mathcal{E}(n)}{\partial w_{ji}(n)}=\frac{\partial\mathcal{E}(n)}{\partial e_{j}(n)}\frac{\partial e_{j}(n)}{\partial y_{j}(n)}\frac{\partial y_{j}(n)}{\partial v_{j}(n)}\frac{\partial v_{j}(n)}{\partial w_{ji}(n)}$$

For output neuron j:
* net internal activity:
	* $v_{j}(n)=\sum_{i=0}^{p}w_{ji}(n)y_{i}(n)$                                                 $\frac{\partial v_{j}(n)}{\partial w_{ji}(n)}=y_{i}(n)$
* output: 
	* $y_{j}(n)=\varphi(v_{j}(n))$                                                              $\frac{\partial y_{j}(n)}{\partial v_{j}(n)}=\varphi^{\prime}(v_{j}(n))$
* error: 
		* $e_{j}(n)=d_{j}(n)-y_{j}(n)$                                                 $\frac{\partial e_{j}(n)}{\partial y_{j}(n)}=-1$
* instantaneous sum of square errors: 
	* $\mathcal{E}(n)=\frac{1}{2}\sum_{j\in C}e_{j}^{2}(n)$                                                       $\frac{\partial\mathcal{E}(n)}{\partial e_{j}(n)}=e_{j}(n)$

Therefore,
# $\frac{\partial\mathcal{E}(n)}{\partial w_{ji}(n)}=-e_{j}(n)\varphi^{\prime}(v_{j}(n))y_{i}(n)$                                         (10)


17/39


# Supplemental: Deriving the Instantaneous Gradient (The Chain Rule)

Slide 17 shows how to calculate the instantaneous gradient: $\frac{\partial\mathcal{E}(n)}{\partial w_{ji}(n)}$. This formula represents how a tiny change in a specific weight ($w_{ji}$) impacts the overall error ($\mathcal{E}$) of the network. 

Because the weight is at the "front" of the neuron's operation and the error is calculated at the "end," we cannot calculate this directly. Instead, we use the **Calculus Chain Rule** to step backward through the neuron's operations, calculating four separate partial derivatives and multiplying them together. 

Here is the step-by-step breakdown of those four parts:

### Step 1: How does the overall error ($\mathcal{E}$) change as the neuron's error signal ($e_j$) changes?
* **Equation:** We know the error for this specific output neuron is $\mathcal{E}(n) = \frac{1}{2} e_j^2(n)$.
* **Derivative:** Using the power rule, the 2 drops down and cancels out the $\frac{1}{2}$. 
* **Result 1:** $\frac{\partial\mathcal{E}(n)}{\partial e_{j}(n)} = e_j(n)$

### Step 2: How does the error signal ($e_j$) change as the actual output ($y_j$) changes?
* **Equation:** The error signal is the target minus the actual output: $e_{j}(n) = d_{j}(n) - y_{j}(n)$.
* **Derivative:** Since the target $d_j(n)$ is a constant, its derivative is 0. The derivative of $-y_j(n)$ with respect to $y_j(n)$ is simply $-1$.
* **Result 2:** $\frac{\partial e_{j}(n)}{\partial y_{j}(n)} = -1$

### Step 3: How does the actual output ($y_j$) change as the net internal activity ($v_j$) changes?
* **Equation:** The output is just the activation function applied to the internal activity: $y_{j}(n) = \varphi(v_{j}(n))$.
* **Derivative:** This is simply the formal derivative of whatever activation function we are using (like the Logistic or Tanh functions discussed later).
* **Result 3:** $\frac{\partial y_{j}(n)}{\partial v_{j}(n)} = \varphi^{\prime}(v_{j}(n))$

### Step 4: How does the net internal activity ($v_j$) change as our specific weight ($w_{ji}$) changes?
* **Equation:** The internal activity is the sum of all inputs multiplied by their weights: $v_{j}(n) = \sum_{i=0}^{p}w_{ji}(n)y_{i}(n)$.
* **Derivative:** We are only taking the derivative with respect to one specific weight, $w_{ji}$. All the other weights in the sum are treated as constants, so they become 0. The derivative of $w_{ji}(n) \cdot y_i(n)$ with respect to $w_{ji}(n)$ leaves only the input value.
* **Result 4:** $\frac{\partial v_{j}(n)}{\partial w_{ji}(n)} = y_{i}(n)$

### Step 5: The Final Chain Rule Assembly
Now, we multiply the four results together to get our final gradient equation:

$$\frac{\partial\mathcal{E}(n)}{\partial w_{ji}(n)} = (\text{Result 1}) \cdot (\text{Result 2}) \cdot (\text{Result 3}) \cdot (\text{Result 4})$$

$$\frac{\partial\mathcal{E}(n)}{\partial w_{ji}(n)} = [e_j(n)] \cdot [-1] \cdot [\varphi^{\prime}(v_{j}(n))] \cdot [y_{i}(n)]$$

By pulling the $-1$ to the front, we arrive at the final equation shown on Slide 17:
$$\frac{\partial\mathcal{E}(n)}{\partial w_{ji}(n)} = -e_j(n)\varphi^{\prime}(v_{j}(n))y_{i}(n)$$
---
# **Navigation**
[[L7B-Slide-16|Previous ← BP Instantaneous Gradient]]
[[AI 201 - Artificial Intelligence/Lecture 7B Backpropagation/L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-18|Next → Local Gradient (Delta)]]
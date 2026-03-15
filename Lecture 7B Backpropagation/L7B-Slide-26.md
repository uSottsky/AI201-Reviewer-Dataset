# The Momentum Term

Small values of the learning rate parameter $\eta$ make the trajectory in weight space smooth.
* learning is slow
* long training time

Too large a value of $\eta$ might make the network unstable because of oscillations.

Speed-up in learning can be achieved without sacrificing stability by including a momentum term in the equation:
# $\Delta w_{ji}(n)=\alpha\Delta w_{ji}(n-1)+\eta\delta_{j}(n)y_{j}(n)$                            (17)

where $\alpha$ is a positive number called the **momentum constant.**

**Generalized Delta Rule.**
* large changes in $w_{ji}$ cause instability because it is based on the local gradient.
* the Generalized Delta Rule takes into account also the value and direction of the previous weight update (and therefore the previous local gradient value).
* when the partial derivative $\partial\mathcal{E}(n)/\partial w_{ji}(n)$ has the same algebraic sign on consecutive iterations, $\Delta w_{ji}(n)$ increases in magnitude so there is an acceleration in the downward direction.
* when the partial derivative $\partial\mathcal{E}(n)/\partial w_{ji}(n)$ has opposite signs on consecutive iterations, $\Delta w_{ji}(n)$ decreases in magnitude so the weight $w_{ji}(n)$ is adjusted by a small amount.
* This stabilizes the network.


26/39



# Supplemental: Understanding the Momentum Term (Slide 26)



Slide 26 introduces a critical enhancement to the basic backpropagation weight update equation: **The Momentum Term**. This solves a common dilemma encountered when choosing a learning rate ($\eta$).

### The Learning Rate Dilemma
When training a neural network using standard gradient descent, you must choose a learning rate ($\eta$):
* **If $\eta$ is too small:** The trajectory through the weight space is smooth, but learning is incredibly slow and training takes a very long time.
* **If $\eta$ is too large:** The network might become unstable and oscillate erratically across the error surface instead of settling into a minimum.

To speed up learning without sacrificing stability, we modify the Generalized Delta Rule by adding a "momentum" term.

---

### The Equation
The updated weight adjustment formula is:
$$\Delta w_{ji}(n) = \alpha \Delta w_{ji}(n-1) + \eta \delta_{j}(n) y_{i}(n)$$
*(Note: The slide contains a slight typographical error where it says $y_j(n)$ at the end of the equation; mathematically, it is multiplied by the input signal $y_i(n)$ from the previous neuron, as established in the standard delta rule on Slide 22).*

**Breaking down the pieces:**
* **$\Delta w_{ji}(n)$**: The new weight adjustment for the current iteration.
* **$\alpha \Delta w_{ji}(n-1)$**: The **Momentum Term**. This takes the exact weight update from the *previous* iteration ($n-1$) and scales it by $\alpha$, a positive number called the momentum constant.
* **$\eta \delta_{j}(n) y_{i}(n)$**: The standard backpropagation gradient step based on the current iteration's error.

---

### How Momentum Works (The Two Scenarios)
By taking into account both the value and the direction of the *previous* weight update, the momentum term acts like physical inertia. It handles two distinct scenarios:

**Scenario 1: Acceleration (Same Sign)**
When the partial derivative $\frac{\partial\mathcal{E}(n)}{\partial w_{ji}(n)}$ has the **same algebraic sign** on consecutive iterations, it means the gradient is consistently pointing in the same direction. 
* Because the current update and the previous update share the same sign, they add together.
* The magnitude of $\Delta w_{ji}(n)$ increases, accelerating the descent down the error surface.

**Scenario 2: Damping / Stabilization (Opposite Signs)**
When the partial derivative $\frac{\partial\mathcal{E}(n)}{\partial w_{ji}(n)}$ has **opposite signs** on consecutive iterations, it means the gradient is oscillating (bouncing back and forth across a valley). 
* Because the current update and the previous update have different signs, they partially cancel each other out.
* The magnitude of $\Delta w_{ji}(n)$ decreases, resulting in a much smaller weight adjustment.

### Conclusion
Large changes in $w_{ji}$ based purely on the local gradient can cause severe instability. By adding the momentum term, the algorithm dampens erratic oscillations while accelerating progress along consistent, smooth gradients, effectively stabilizing the network during training.

---
# **Navigation**
[[L7B-Slide-25|Previous ← Hyperbolic Tangent Nonlinearity]]
[[AI 201 - Artificial Intelligence/Lecture 7B Backpropagation/L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-27|Next → Pattern and Batch Training]]
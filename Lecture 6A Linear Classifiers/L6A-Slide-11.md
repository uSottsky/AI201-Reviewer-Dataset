# Perceptron

### The Perceptron Algorithm
For iterative minimization of the cost function, adopt an iterative scheme in the spirit of gradient descent:
$$w(t+1) = w(t) - \rho_t \frac{\partial J(w)}{\partial w} \bigg|_{w=w(t)}$$

where $w(t)$ is the weight vector estimate at the $t^{th}$ iteration step and $\rho_t$ is a sequence of positive real numbers.
At points where $J(w)$ is valid, we have $\frac{\partial J(w)}{\partial w} = \sum_{x \in Y} \delta_x x$ so that:
$$w(t+1) = w(t) - \rho_t \sum_{x \in Y} \delta_x x$$

**Perceptron Algorithm**
1. choose $w(0)$ randomly
2. choose $\rho_0$
3. $t=0$
4. repeat
   * $Y = \emptyset$ (set of misclassified points)
   * for $i=1$ to $N$
     * if $\delta_{x_i} w(t)^T x_i \ge 0$ then $Y = Y \cup \{x_i\}$
   * $w(t+1) = w(t) - \rho_t \sum_{x \in Y} \delta_x x$
   * adjust $\rho_t$
   * $t = t+1$
   * until $Y = \emptyset$

---
**Navigation**
[[L6A-Slide-10|Previous ← Computing Unknown Parameters]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-12|Next → Geometric Interpretation]]
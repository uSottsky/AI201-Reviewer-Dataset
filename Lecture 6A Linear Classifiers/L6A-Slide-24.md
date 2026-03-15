# LMS Algorithm

### The LMS (Widrow-Hoff) Algorithm
For the iteration scheme that solves Eqn 4, Eqn 6 becomes:
$$\hat{w}(k) = \hat{w}(k-1) + \rho_k x_k (y_k - x_k^T \hat{w}(k-1)) \quad \text{(7)}$$

where $(y_k, x_k)$ are the desired output $(\pm 1)$ - input training sample pairs successively presented to the algorithm. This algorithm converges asymptotically to the MSE solution.

A common variant is to use a constant $\rho$ in place of $\rho_k$.
It can be shown that if $0 < \rho < 2/tr[R_x]$ then the mean value of the LMS estimate is equal to the MSE solution and the corresponding variance remains finite.
* smaller $\rho$ yields smaller variance around MSE solution
* smaller $\rho$ results in slower convergence
* constant $\rho$ can track variations when the statistics are not stationary (slowly varying), i.e., when the underlying distributions are time dependent.

the parameters' update iteration step $k$ coincides with the index of the current input sample $x_k$.
* If $k$ is a time index, LMS is time-adaptive (i.e., it adapts to the solution as successive samples become available to the system)

Equation 7 can be seen as the training algorithm for a linear neuron (one without the nonlinear activation function).
This neuron is known as the **adaline** (adaptive linear element) used by Widrow and Hoff. The adaline is a neuron trained according to the LMS instead of the perceptron algorithm.

---
**Navigation**
[[L6A-Slide-23|Previous ← Stochastic Approximation]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-25|Next → Sum of Error Squares Estimation]]
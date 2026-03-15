# Mean Square Error Estimation

Minimizing $J(w)$ leads to:
$$\frac{\partial J(w)}{\partial w} = 2E[x(y - x^T w)] = 0 \quad \text{(4)}$$
$$\hat{w} = R_x^{-1} E[xy] \quad \text{(5)}$$

where $R_x$ is the correlation matrix and is equal to the covariance matrix if the respective mean values are zero:
$$R_x \equiv E[x x^T] = \begin{bmatrix} E[x_1 x_1] & \cdots & E[x_1 x_l] \\ E[x_2 x_1] & \cdots & E[x_2 x_l] \\ \vdots & \vdots & \vdots \\ E[x_l x_1] & \cdots & E[x_l x_l] \end{bmatrix}$$

The cross-correlation between the desired output and the input feature vectors is:
$$E[xy] = E \begin{bmatrix} x_1 y \\ \vdots \\ x_l y \end{bmatrix}$$

The mean square optimal weight vector is the solution to the linear set of equations provided that the correlation matrix is invertible.

---
**Navigation**
[[L6A-Slide-19|Previous ← Mean Square Error Estimation]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-21|Next → Mean Square Error Estimation (Geometric View)]]
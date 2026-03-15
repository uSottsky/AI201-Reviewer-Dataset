# Sum of Error Squares Estimation

### Sum of Error Squares Estimation
Another criterion closely related to the MSE: sum of error squares (aka least squares (LS)) criterion:
$$J(w) = \sum_{i=1}^N (y_i - x_i^T w)^2 \equiv \sum_{i=1}^N e_i^2 \quad \text{(8)}$$

Errors between desired output of classifier (e.g., $\pm 1$ for 2 classes) and true output are summed up over all available training feature vectors, instead of averaging them. This does not need explicit knowledge of the underlying pdfs. Minimizing eqn 8 wrt $w$ yields:
$$\sum_{i=1}^N x_i (y_i - x_i^T \hat{w}) = 0 \Rightarrow \left( \sum_{i=1}^N x_i x_i^T \right) \hat{w} = \sum_{i=1}^N (x_i y_i) \quad \text{(9)}$$

Define $X$ to be the $N \times l$ matrix whose rows are the available training feature vectors and $y$ is the vector of labels:
$$X = \begin{bmatrix} x_1^T \\ x_2^T \\ \vdots \\ x_N^T \end{bmatrix} = \begin{bmatrix} x_{11} & x_{12} & \cdots & x_{1l} \\ x_{21} & x_{22} & \cdots & x_{2l} \\ \vdots & \vdots & \vdots & \vdots \\ x_{N1} & x_{N2} & \cdots & x_{Nl} \end{bmatrix}, \quad y = \begin{bmatrix} y_1 \\ y_2 \\ \vdots \\ y_N \end{bmatrix}$$

From Eqn 9 we obtain:
$$\hat{w} = (X^T X)^{-1} X^T y = X^+ y$$
Optimal weight vector is the product of the pseudoinverse of $X$ and the sample class labels.

---
**Navigation**
[[L6A-Slide-24|Previous ← The LMS (Widrow-Hoff) Algorithm]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-26|Next → Mean Square Error Regression]]
# Mean Square Error Estimation

### Multiclass Case
Task: design the $M$ linear discriminant functions $g_i(x) = w_i^T x$ according to the MSE criterion.
Desired output responses (i.e., class labels) are chosen so that $y_i = 1$ if $x \in \omega_i$ and $y_i = 0$ otherwise.

Define $y^T = [y_1, y_2, ..., y_M]$ for a given vector $x$ and $W = [w_1, w_2, ..., w_M]$. Following the MSE criterion, minimize the norm of the error vector $y - W^T x$, i.e.,
$$\hat{W} = \arg \min_W E[||y - W^T x||^2] = \arg \min_W \left[ \sum_{i=1}^M E[(y_i - w_i^T x)^2] \right]$$

This is equivalent to $M$ MSE independent minimization problems of the type we discussed.
Thus, in order to design the MSE optimal linear discriminant functions, it suffices to design each one of them so that its desired output is 1 for vectors belonging to the corresponding class and 0 for all the others.

---
**Navigation**
[[L6A-Slide-21|Previous ← Mean Square Error Estimation (Geometric View)]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-23|Next → Stochastic Approximation]]
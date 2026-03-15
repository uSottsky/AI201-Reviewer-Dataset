# Perceptron

### Geometric Interpretation



$$w(t+1) = w(t) - \rho_t \sum_{x \in Y} \delta_x x$$


![[Pasted image 20260315214810.png]]
> Reference: Slide 12 - Vector plot showing the geometric interpretation of the Perceptron update rule. A misclassified vector $x$ causes the weight vector $w(t)$ to be adjusted towards $w(t+1)$.



Misclassified example $x$ at time $t$ where $\rho_t=1$.
Perceptron algorithm corrects the weight vector in the direction of $x$. The decision hyperplane is reoriented so that $x$ is classified in the correct class $\omega_1$.

---
**Navigation**
[[L6A-Slide-11|Previous ← The Perceptron Algorithm]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-13|Next → Perceptron Convergence Theorem]]
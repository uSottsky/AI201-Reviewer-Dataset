# Optimization Review

### Gradient Descent Algorithm

![[Pasted image 20260315214314.png]]
> Reference: Slide 3 - Graph of Gradient Descent showing parameter $\theta$ updates moving down the slope towards the minimum of $J(\theta)$.

Let $\theta$ be an unknown parameter vector and $J(\theta)$ the corresponding cost function to be minimized. Assume that $J(\theta)$ is differentiable.

**Gradient Descent Algorithm**
Gradient descent starts with initial estimate $\theta(0)$ of the minimum point.
Subsequent iterations are of the form:
$$\theta(new) = \theta(old) + \Delta\theta$$
$$\Delta\theta = -\mu \frac{\partial J(\theta)}{\partial\theta} \bigg|_{\theta=\theta(old)}$$

where $\mu > 0$. If the maximum is sought, the method is known as gradient ascent and the minus is removed.
* new estimate $\theta(new)$ chosen in the direction that decreases $J(\theta)$

---
**Navigation**
[[L6A-Slide-02|Previous ← Outline]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-04|Next → Gradient Descent Convergence]]
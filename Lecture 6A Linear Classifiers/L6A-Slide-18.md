# Perceptron

### The Pocket Algorithm
Perceptron Algorithm will not converge if data is not linearly separable.
The Pocket Algorithm is a variant of the Perceptron Algorithm that converges to an optimal solution even when the linear separability condition is not satisfied.

**Pocket Algorithm**
1. Initialize weight vector $w(0)$ randomly. Define a stored vector $w_s$. Set history counter $h_s$ of $w_s$ to zero.
2. At the $t^{th}$ iteration, compute update $w(t+1)$ according to the perceptron rule.
3. Use updated weight vector to test the number $h$ of training vectors that are classified correctly.
4. If $h > h_s$ replace $w_s$ with $w(t+1)$ and $h_s$ with $h$. Continue the iterations.

It can be shown that the Pocket Algorithm converges with probability one to the optimal solution – the one that produces the minimum number of misclassifications.

---
**Navigation**
[[L6A-Slide-17|Previous ← The Perceptron Network]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-19|Next → Mean Square Error Estimation]]
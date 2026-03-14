# Backpropagation Algorithm Derivation
![[Pasted image 20260314211632.png]]

We defined the instantaneous sum of squared errors as
# $\mathcal{E}(n)=\frac{1}{2}\sum_{k\in C}e_{k}^{2}(n)$
# $\frac{\partial\mathcal{E}(n)}{\partial y_{j}(n)}=\sum_{k\in C}e_{k}(n)\frac{\partial e_{k}(n)}{\partial y_{j}(n)}$

which, after using the chain rule, becomes

# $\frac{\partial\mathcal{E}(n)}{\partial y_{j}(n)}=\sum_{k\in C}e_{k}(n)\frac{\partial e_{k}(n)}{\partial v_{k}(n)}\frac{\partial v_{k}(n)}{\partial y_{j}(n)}$

However,
# $e_{k}(n)=d_{k}(n)-y_{k}(n)$
# $=d_{k}(n)-\varphi(v_{k}(n))$

so that
# $\frac{\partial e_{k}(n)}{\partial v_{k}(n)}=-\varphi^{\prime}(v_{k}(n))$

Note also that
# $\frac{\partial v_{k}(n)}{\partial y_{j}(n)}=w_{kj}(n)$      since          $v_{k}(n)=\sum_{j=0}^{q}w_{kj}(n)y_{j}(n)$


20/39

# Supplemental: Step-by-Step Calculus for Network Derivatives

Backpropagation relies on chaining fundamental derivative terms. Here is the step-by-step calculus showing exactly how the structural derivatives (error, cost, and internal activity) are solved.

---

## 1. The Error term derivative: $\frac{\partial e_j(n)}{\partial y_j(n)}$
**The Equation:** The error is the desired target minus the actual output.
### $$e_j(n) = d_j(n) - y_j(n)$$

**The Steps:**
1. We take the derivative with respect to the output, $y_j(n)$.
2. The target, $d_j(n)$, is a fixed constant for a given training pattern. The derivative of a constant is $0$.
3. The derivative of $-y_j(n)$ with respect to $y_j(n)$ is just $-1$ (using the power rule: $-1 \cdot y_j^{1-1} = -1 \cdot 1 = -1$).

**Result:** $$\frac{\partial e_j(n)}{\partial y_j(n)} = 0 - 1 = -1$$

---

## 2. The Cost Function derivative: $\frac{\partial\mathcal{E}(n)}{\partial e_j(n)}$
**The Equation:** The instantaneous squared error for a single neuron.
### $$\mathcal{E}(n) = \frac{1}{2} e_j^2(n)$$

**The Steps:**
1. We take the derivative with respect to the error, $e_j(n)$.
2. Using the standard Power Rule of calculus ($d/dx[x^n] = n \cdot x^{n-1}$), the exponent $2$ drops down to the front.
3. The exponent becomes $2 - 1 = 1$.
4. We multiply the dropped $2$ by the $\frac{1}{2}$ at the front.
### $$\frac{\partial\mathcal{E}(n)}{\partial e_j(n)} = \left(\frac{1}{2} \cdot 2\right) \cdot e_j^1(n)$$

### **Result:** $$\frac{\partial\mathcal{E}(n)}{\partial e_j(n)} = e_j(n)$$

---

## 3. The Internal Activity (Linear Combiner) derivatives
**The Equation:** The net internal activity is the sum of all inputs times their weights.
### $$v_j(n) = w_{j0}y_0 + w_{j1}y_1 + \dots + w_{ji}y_i + \dots + w_{jp}y_p$$

**Derivative A: With respect to a specific weight ($w_{ji}$)**
1. We want to see how $v_j$ changes if we *only* change a specific weight, $w_{ji}$.
2. All other terms in the sum (like $w_{j1}y_1$) are treated as constants. The derivative of a constant is $0$.
3. We are left only deriving the specific term $w_{ji}y_i$ with respect to $w_{ji}$.
4. Since $y_i$ is treated as a constant coefficient attached to $w_{ji}$, the derivative is just $y_i$.

## **Result:** $$\frac{\partial v_j(n)}{\partial w_{ji}(n)} = y_i(n)$$

**Derivative B: With respect to a specific input ($y_j$) (Used in Hidden Layers)**
1. Let's look at the next layer's activity:
### $$v_k = \sum w_{kj}y_j$$
1. We want to see how $v_k$ changes if we *only* change the incoming signal from the previous layer, $y_j$.
2. All other terms in the sum become $0$.
3. Deriving $w_{kj}y_j$ with respect to $y_j$ leaves only the constant coefficient, $w_{kj}$.

## **Result:** $$\frac{\partial v_k(n)}{\partial y_j(n)} = w_{kj}(n)$$

---
# **Navigation**
[[L7B-Slide-19|Previous ← Case 2: Hidden Neuron]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-21|Next → Hidden Neuron Delta]]
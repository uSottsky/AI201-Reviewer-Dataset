# Example (SAT Scores and Passing a Course)



Logistic Regression Model: $p(y_{i}=1|x_{i},w) = sigmoid(w_{0}+w_{1}x_{i})$ where $X_{i}$ is the SAT score of student $i$ and $y_{i}$ is whether the student passed or failed the class.

![[Pasted image 20260315164935.png]]
> Reference: Slide 17 - Scatter plot showing SAT scores (x-axis) vs Pass/Fail (y-axis at 0 and 1). Black dots represent training data. Red circles represent the probabilities mapped by the estimated sigmoid function.
* **black:** training data
* **red:** $p(y_{i}=1|x_{i},\hat{w})$, where $\hat{w}$ is estimated from training data

Threshold at $p=0.5$ induces the decision rule:
$$\hat{y}(x)=1 \Leftrightarrow p(y=1|x)>0.5$$

Decision rule has a non-zero error rate even in the training set because data is not linearly separable (no straight line that can separate the 0's from the 1's).

17/25

---
**Navigation**
[[L5A-Slide-16|Previous ← Logistic Regression Equation]]
[[L5A-0-Table-of-Contents|↑ Lecture 5A TOC]]
[[L5A-Slide-18|Next → Overfitting (Regression)]]
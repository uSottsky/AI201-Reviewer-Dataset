# Heuristics for Making the BP Algorithm Perform Better


1. **Pattern vs Batch Update**
* Pattern mode is faster than batch mode

**Activation Function**
* hyperbolic tangent function is better than logistic function
# * $\varphi(v)=a~tanh(bv)$
# * $\varphi^{\prime}(v)=\frac{b}{a}[a-\varphi(v)^{2}][a+\varphi(v)]$
# * where $a=1.716$ and $b=\frac{2}{3}$.


> ![[Pasted image 20260314213851.png]]
> Reference: Slide 31 - Graph showing the Hyperbolic Tangent Function curve with intercepts marked at $a=1.7159$.


**Target Values**
* desired output of neuron should be offset by some amount e away from limiting value


31/39

---
**Navigation**
[[L7B-Slide-30|Previous ← Backpropagation Algorithm Steps 4-10]]
[[AI 201 - Artificial Intelligence/Lecture 7B Backpropagation/L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-32|Next → Heuristics (Data Normalization)]]
# The Momentum Term

Small values of the learning rate parameter $\eta$ make the trajectory in weight space smooth.
* learning is slow
* long training time

Too large a value of $\eta$ might make the network unstable because of oscillations.

Speed-up in learning can be achieved without sacrificing stability by including a momentum term in the equation:
# $\Delta w_{ji}(n)=\alpha\Delta w_{ji}(n-1)+\eta\delta_{j}(n)y_{j}(n)$                            (17)

where $\alpha$ is a positive number called the **momentum constant.**

**Generalized Delta Rule.**
* large changes in $w_{ji}$ cause instability because it is based on the local gradient.
* the Generalized Delta Rule takes into account also the value and direction of the previous weight update (and therefore the previous local gradient value).
* when the partial derivative $\partial\mathcal{E}(n)/\partial w_{ji}(n)$ has the same algebraic sign on consecutive iterations, $\Delta w_{ji}(n)$ increases in magnitude so there is an acceleration in the downward direction.
* when the partial derivative $\partial\mathcal{E}(n)/\partial w_{ji}(n)$ has opposite signs on consecutive iterations, $\Delta w_{ji}(n)$ decreases in magnitude so the weight $w_{ji}(n)$ is adjusted by a small amount.
* This stabilizes the network.


26/39

---
**Navigation**
[[L7B-Slide-25|Previous ← Hyperbolic Tangent Nonlinearity]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-27|Next → Pattern and Batch Training]]
# Stopping Criterian

 
Let the weight vector $w^{*}$ denote a local or global minimum.
We have the following criteria for terminating training:

1. **Property of a minimum:** The gradient at $w^{*}$ is zero.
    * **Criterion:** The backpropagation algorithm is considered to have converged when the Euclidean norm of the gradient vector reaches a sufficiently small gradient threshold.
	    * **drawback:** requires calculation of the gradient vector $g(w)$ which is computationally expensive
2. **Property of a minimum:** Cost function $\mathcal{E}_{av}(w)$ does not change at $w=w^{*}$.
    * **Criterion:** The backpropagation algorithm is considered to have converged when the absolute rate of change in the average squared error per epoch is sufficiently small (0.1% to 1% per epoch).
3. **Cost function** $\mathcal{E}_{av}(w)$ must be less than or equal to a sufficiently small threshold.
    * **Criterion:** The backpropagation algorithm is considered to have converged when the average squared error per epoch is sufficiently small.
4. **Combination of 1 and 3.**
    * **Criterion:** The backpropagation algorithm is terminated at the weight vector $w_{final}$ when $||g(w_{final})||\le\epsilon,$ where $\epsilon$ is a sufficiently small gradient threshold, or when $\mathcal{E}_{av}(w_{final})\le\tau$, where $\tau$ is a sufficiently small error energy threshold.

After each learning iteration, the network is tested for its generalization performance. Training stops when the generalization performance is adequate or when it is apparent that it has peaked.


28/39

---
**Navigation**
[[L7B-Slide-27|Previous ← Pattern and Batch Training]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-29|Next → Backpropagation Algorithm Steps 1-3]]
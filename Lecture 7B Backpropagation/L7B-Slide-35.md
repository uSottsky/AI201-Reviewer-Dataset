# Convergence

**Backpropagation Algorithm**
* performs a gradient descent search through the space of possible network weights (weight space)
* error surface for MLP may contain many local minima so that gradient descent search can become trapped in any of them
* BP is guaranteed to converge toward some local minima and not necessarily to the global minimum

A network with a large number of weights will have an error surface in very high dimensional space (one dimension per weight)
* when gradient descent falls into a local minimum with respect to one of the weights, it will not necessarily be in the local minimum with respect to the other weights
* the more weights the network has, the more dimensions there are that might provide "escape routes" for gradient descent to fall away from the local minimum with respect to this single weight

Consider the way the network weights evolve as the number of training iteration increases
* if the network weights are initialized to values near zero, then at the early phase of training, the network will represent a very smooth function that is approximately linear in its inputs
* sigmoid activation function is itself approximately linear when the weights are close to zero.
* as the number of training iterations increases, the weights evolve so that at some point they can represent highly nonlinear functions.

35/39

---
**Navigation**
[[L7B-Slide-34|Previous ← Decision Rule]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-36|Next → Generalization]]
# Backpropagation Algorithm Derivation

### Backpropagation Algorithm
**Initialization**
1. Configure the network (determine the number of hidden layers and number of nodes in each hidden and output layers)
2. Initialize the synaptic weights and biases to small uniformly distributed random numbers
3. Present the network with an epoch of training examples
For each training example, $[x(n), d(n)]$, perform steps 3 to 10:

**Forward Computation**
4. Apply the input vector $x(n)$ to the input layer.
    * $x_{j}(n)$ is the $j$th element of the input vector $x(n)$
    * for layer 1 (input layer), $y_{j}^{(0)}(n)=x_{j}(n)$
5. Calculate the activation potentials of the neurons in the layers $l$:
    * $v_{j}^{(l)}(n)=\sum_{i=0}^{m}w_{ji}^{(l)}(n)y_{i}^{(l-1)}(n)$
    * for $i=0$ , we have $y_{0}^{(l-1)}(n)=1$ and $w_{j0}^{(l)}(n)$ is treated just like the other weights.
6. Calculate the outputs for the layer $l$:
    * $y_{j}^{(l)}(n)=\varphi(v_{j}^{(l)}(n))=\frac{1}{1+e^{-v_{j}^{(l)}(n)}}$        (logistic activation)


29/39

---
**Navigation**
[[L7B-Slide-28|Previous ← Stopping Criteria]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-30|Next → Backpropagation Algorithm Steps 4-10]]
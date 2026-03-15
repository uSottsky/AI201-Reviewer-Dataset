# The Multi-layer Perceptron

### Representational Power of Feedforward Networks
Feedforward networks are capable of representing:

**Boolean Functions**
* every boolean function can be represented exactly by some network with one hidden layer
* For each possible input vector, associate a distinct hidden neuron and set its weights so that it activates if and only if this specific vector is input to the network.
* the hidden layer will always have exactly one neuron that fires
* implement the output neuron as an OR gate that activates only for the desired input patterns
* number of hidden neurons required to implement boolean function grows exponentially (in the worst case) with the number of network inputs

**Continuous Functions**
* Every bounded continuous function can be approximated with arbitrarily small error by a network with one hidden layer (Cybenko, 1989)
* required number of neurons in the hidden layer depends on the function to be approximated

**Arbitrary Functions**
* Any function can be approximated to arbitrary accuracy by a network with two hidden layers
* number of neurons at each layer is, in general, not known

---
**Navigation**
[[L7A-Slide-34|Previous ← Three-Layer Perceptron]]
[[L7A-0-Table-of-Contents|↑ Lecture 7A TOC]]
[[L7A-Slide-36|Next → Universal Approximation Theorem]]
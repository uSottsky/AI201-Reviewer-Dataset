# The Multi-layer Perceptron

### Three-Layer Perceptron


The Three-Layer Perceptron can separate classes resulting from any union of polyhedral regions.

First layer neurons form hyperplanes. Second layer neurons form polyhedral regions. Output layer neurons form classes.


![[Pasted image 20260316030929.png]]
> Reference: Slide 34 - Diagram of a Three-Layer Perceptron. Input nodes connect to a first hidden layer, which connects to a second hidden layer, which finally connects to a single output node.



* **First Layer:** $p$ neurons map input space onto unit hypercube vertices
* **Second Layer:** Class A consists of union of $K$ polyhedra and class B for the rest
  * neurons realize hyperplanes in $p$-dimensional space
  * synaptic weights chosen so that each hyperplane leaves one vertex on one side and all the rest on the other;
  * for each neuron a different vertex is isolated (i.e., one of the $K$ A class vertices)
  * when a class A input vector enters the network, one of the $K$ neurons in 2nd layer produces a 1 and other $K-1$ give a 0
  * when a class B input vector enters a network, all neurons in 2nd layer output a 0
* **Output Layer:** realize an OR gate that outputs a 1 for class A and 0 for class B vectors

---
**Navigation**
[[L7A-Slide-33|Previous ← Polyhedral Regions]]
[[L7A-0-Table-of-Contents|↑ Lecture 7A TOC]]
[[L7A-Slide-35|Next → Representational Power of Feedforward Networks]]
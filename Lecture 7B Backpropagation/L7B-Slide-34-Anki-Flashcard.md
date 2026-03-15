# Anki Flashcard: Decision Rule for MLP

**Q:** What is the decision rule for classifying a pattern in a trained multilayer perceptron (MLP)?

**A:** Assign the input vector $x$ to class $C_k$ if the corresponding output $F_k(x)$ is greater than or equal to $F_j(x)$ for all $j \ne k$, where $F_k(x)$ is the output of the network for class $k$. This means $x$ is classified into the class with the highest output value from the network. If using a fixed threshold (e.g., 0.5), this could lead to multiple class assignments, so the "maximum output" rule is preferred.

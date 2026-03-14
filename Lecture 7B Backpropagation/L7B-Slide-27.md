# Pattern and Batch Training Modes

During training, the order of presentation of training examples must be randomized from one epoch to the next.

Two Ways of Training MLP:
1. **Pattern Mode** - update weights after presentation of each training example.
    * requires less storage
2. **Batch Mode** - update weights after presentation of all training examples (i.e. at the end of each epoch)
    * $\Delta w_{ji}$ is a more accurate estimate of the gradient vector
    * parallelizable


27/39

---
**Navigation**
[[L7B-Slide-26|Previous ← The Momentum Term]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-28|Next → Stopping Criteria]]
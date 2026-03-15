Heuristics for Making the BP Algorithm Perform Better

**Normalize the inputs**

![[Pasted image 20260314214152.png]]
> Reference: Slide 32 - Sequence of 4 scatter plots showing data normalization process: Original set -> Mean removal -> Decorrelation -> Covariance equalization.



* input variables should be uncorrelated (use PCA)
* decorrelated input variables should be scaled so that their covariances are approximately equal
* process each input variable so that its mean value, averaged over the entire training samples is close to zero

32/39

---
**Navigation**
[[L7B-Slide-31|Previous ← Heuristics (Activation & Target)]]
[[AI 201 - Artificial Intelligence/Lecture 7B Backpropagation/L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-33|Next → Other Heuristics]]
# Logistic Discrimination

Let $\theta$ be the vector of unknown parameters and $x_k, k=1,2,...,N$ be the training feature vectors with known class labels. Denote by $x_k^{(m)}, k=1,2,...,N_m$ the vectors originating from class $m=1,2,...,M$. The log-likelihood function to be optimized is:
$$L(\theta) = \ln \left\{ \prod_{k=1}^{N_1} p(x_k^{(1)}|\omega_1; \theta) \prod_{k=1}^{N_2} p(x_k^{(2)}|\omega_2; \theta) \cdots \prod_{k=1}^{N_M} p(x_k^{(M)}|\omega_M; \theta) \right\} \quad \text{(10)}$$

Since:
$$p(x_k^{(m)}|\omega_m; \theta) = \frac{p(x_k^{(m)}) P(\omega_m|x_k^{(m)}; \theta)}{P(\omega_m)}$$

we then have:
$$L(\theta) = \sum_{k=1}^{N_1} \ln P(\omega_1|x_k^{(1)}) + \sum_{k=1}^{N_2} \ln P(\omega_2|x_k^{(2)}) + \cdots + \sum_{k=1}^{N_M} \ln P(\omega_M|x_k^{(M)}) + C \quad \text{(11)}$$

where $C$ is a parameter independent on $\theta$:
$$C = \ln \frac{\prod_{k=1}^N p(x_k)}{\prod_{m=1}^M P(\omega_m)^{N_m}}$$

Any optimization algorithm can be used to perform the maximization of $L(\theta)$ in Eqn 11.

---
**Navigation**
[[L6A-Slide-29|Previous ← Logistic Discrimination]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-31|Next → Logistic Discrimination and LDA]]
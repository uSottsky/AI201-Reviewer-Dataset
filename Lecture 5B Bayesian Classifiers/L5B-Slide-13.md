# Risk Minimization

Minimize a modified version containing penalty terms:

$$
r = \lambda_{12}P(x \in R_2|\omega_1)P(\omega_1) + \lambda_{21}P(x \in R_1|\omega_2)P(\omega_2) 
= \lambda_{12}P(\omega_1) \int_{R_2} p(x|\omega_1)dx + \lambda_{21}P(\omega_2) \int_{R_1} p(x|\omega_2)dx
$$

Consider an M class problem. Let $R_j$ be the regions assigned to class $\omega_j$ for $j = 1, 2, \dots, M$. Suppose a feature vector $x$ that belongs to class $\omega_k$ lies in $R_i$, $i \neq k$. This vector is misclassified as $\omega_i$. A penalty term $\lambda_{ki}$ known as **loss**, is associated with this wrong decision. We can form a loss matrix for the penalty terms $\lambda_{ki}$. The risk or loss associated with $\omega_k$ is defined as

$$
r_k = \sum_{i=1}^{M} \lambda_{ki} \int_{R_i} p(x|\omega_k)dx
$$

The integral is the overall probability of a feature vector from class $\omega_k$ being classified as $\omega_i$. This probability is weighted by $\lambda_{ki}$. We now partition the regions $R_j$ so that the average risk $r$ is minimized:

$$
r = \sum_{k=1}^{M} r_k P(\omega_k) 
= \sum_{i=1}^{M} \int_{R_i} \left( \sum_{k=1}^{M} \lambda_{ki} p(x|\omega_k) P(\omega_k) \right) dx
$$

This is achieved if each of the integrals is minimized which is equivalent to selecting regions so that

$$
x \in R_i \quad \text{if} \quad 
l_i \equiv \sum_{k=1}^{M} \lambda_{ki} p(x|\omega_k) P(\omega_k) 
< l_j \equiv \sum_{k=1}^{M} \lambda_{kj} p(x|\omega_k) P(\omega_k) \quad \forall j \neq i.
$$

 ---
 

13/44

[[L5B-Slide-12|Previous ← M Class Bayesian Classifier]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-14|Next → Two-Class Case]]
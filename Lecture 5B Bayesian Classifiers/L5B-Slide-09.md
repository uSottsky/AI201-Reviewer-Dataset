# Bayes Classification Rule

$$
P(\omega_1|x) > P(\omega_2|x): \text{ classify } x \text{ as } \omega_1
$$

$$
P(\omega_1|x) < P(\omega_2|x): \text{ classify } x \text{ as } \omega_2
$$

(in case of equality, $x$ can be classified as $\omega_1$ or $\omega_2$)

**Rewrite as**

$$
p(x|\omega_1)P(\omega_1) > p(x|\omega_2)P(\omega_2): \text{ classify } x \text{ as } \omega_1
$$

$$
p(x|\omega_1)P(\omega_1) < p(x|\omega_2)P(\omega_2): \text{ classify } x \text{ as } \omega_2
$$

**For equiprobable classes** (i.e., $P(\omega_1) = P(\omega_2)$):

**Classification rule:**

$$
p(x|\omega_1) > p(x|\omega_2): \text{ classify } x \text{ as } \omega_1
$$

$$
p(x|\omega_1) < p(x|\omega_2): \text{ classify } x \text{ as } \omega_2
$$

--- 

9/44

[[L5B-Slide-08|Previous ← Bayes Decision Theory]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-10|Next → Equiprobable Classes]]
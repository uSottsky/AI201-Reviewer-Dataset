# Stochastic Games

> ![[Pasted image 20260315010351.png]]
> Reference: Slide 32 - Expectiminimax tree diagram incorporating CHANCE nodes between MAX and MIN layers, labeled with probabilities like 1/36 (1-1 roll), 1/18 (1-2 roll), etc.

### Expectiminimax

$$
Expectiminimax(s) = 
\begin{cases} 
Utility(s, Max) & \text{if } IsTerminal(s) \\ 
\max_a \in Actions(s) Expectiminimax(Result(s,a)) & \text{if } ToMove(s) = Max \\ 
\min_a \in Actions(s) Expectiminimax(Result(s,a)) & \text{if } ToMove(s) = Min \\
\sum_r P(r) Expectiminimax(Result(s,r)) & \text{if } ToMove(s) = Chance 
\end{cases}
$$

- $r$ represents a possible dice roll and $Result(s,r)$ is the same as state $s$ with additional fact that it is the result of the dice roll


32/34

---
**Navigation**
[[L3C-Slide-31|Previous ← Stochastic Games (Backgammon)]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-33|Next → Evaluation Functions for Games of Chance]]
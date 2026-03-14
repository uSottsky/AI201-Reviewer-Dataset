# Mini-Max

### Minimax Optimal Strategy

$$
Minimax(s) = 
\begin{cases} 
Utility(s, Max) & \text{if } IsTerminal(s) \\ 
\max_{a \in Actions(s)} Minimax(Result(s, a)) & \text{if } ToMove(s) = Max \\ 
\min_{a \in Actions(s)} Minimax(Result(s, a)) & \text{if } ToMove(s) = Min 
\end{cases}
$$

* Minimax decision assumes that the opponent will play perfectly
* if max depth of tree is $m$, and there are $b$ legal moves for each node, the time complexity of minimax is $O(b^m)$, which makes this algorithm impractical
* space complexity is linear in $m$ and $b$ since minimax is depth-first search
 
10/34

---
**Navigation**
[[L3C-Slide-09|Previous ← Mini-Max: Tic-Tac-Toe Tree]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-11|Next → Minimax Algorithm Steps]]
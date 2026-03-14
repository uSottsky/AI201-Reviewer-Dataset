# Multiplayer Games

### Mini-Max

![[Pasted image 20260315004920.png]]
> Reference: Slide 12 - A multiplayer game tree for 3 players (A, B, C) where each node contains a vector of values like (1, 2, 6).

* each node returns a vector of values $(e.g., [v_a, v_b, v_c])$
* terminal states: utility of state from each player's viewpoint
* backed-up value of a node $n$ is the utility vector of the successor state with the highest value for the player choosing at $n$

 
12/34

---
**Navigation**
[[L3C-Slide-11|Previous ← Minimax Algorithm Steps]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-13|Next → Chess: Rules & Objective]]
# Alpha-Beta Pruning

![[Pasted image 20260315005102.png]]
> Reference: Slide 16 - Abstract game tree showing a Player at node m, passing to Opponent, who passes to Player at node n. A wavy dashed line connects node m to a later descendant node n to illustrate pruning conditions.

Player has a choice in moving to node $n$. If Player has a better choice either at the same level ($m^{\prime}$) or at any point higher up in the tree ($m$), then Player will never move to $n$.

Prune tree at node $n$.

 
16/34

---
**Navigation**
[[L3C-Slide-15|Previous ← Alpha-Beta Pruning Example]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-17|Next → Alpha and Beta Definitions]]
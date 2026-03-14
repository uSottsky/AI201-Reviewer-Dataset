# Alpha-Beta Pruning

![[Pasted image 20260315005035.png]]
> Reference: Slide 15 - Minimax tree showing Alpha-Beta pruning in action. The root node A is [3, 3]. Node B evaluates to 3. Node C evaluates to 2 and its remaining children are pruned (dashed lines). Node D evaluates to 2.

$$Minimax(root) = \max(\min(3,12,8), \min(2,x,y), \min(14,5,2))$$
$$= \max(3, \min(2,x,y), 2)$$
$$= \max(3, z, 2) \text{ where } z = \min(2,x,y) \le 2$$
$$= 3$$

 
15/34

---
**Navigation**
[[L3C-Slide-14|Previous ← Imperfect Decisions]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-16|Next → Alpha-Beta Pruning Concept]]
# A* Search

$A^{*}$ Search
$A^{*}$ search minimizes the total path cost
Let $f(n)=g(n)+h(n)$
		= path cost from start node to node n
		+ estimated cost of the cheapest path from n to goal
		= estimated cost of the cheapest solution through n

**function** $A^{*}$ -Search(problem) returns solution or failure
	**return** BEST-FIRST-SEARCH(problem, $g+h)$

$A^{*}$ **is complete and optimal if h never overestimates the cost to reach the goal, i.e.**
$h(n)\le$ actual distance from node n to goal

10/25

---
**Navigation** [[L3B-Slide-09|Previous ← Greedy Search Complexity]]  
[[L3B-0-Table-of-Contents|↑ Lecture 3B TOC]]  
[[L3B-Slide-11|Next → Admissible Heuristic]]
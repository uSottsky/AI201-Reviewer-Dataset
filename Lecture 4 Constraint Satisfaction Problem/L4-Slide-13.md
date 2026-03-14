# CSP as a search problem

![[Pasted image 20260315013902.png]]
> Reference: Slide 13 - Continuation of the map coloring search tree.

### CSP as Search
* **Initial state:** empty assignment
* **Successor function:** assign a value to unassigned variable
* **Goal Test:** complete assignment where all constraints are satisfied

**Assignments are commutative:**
$[WA=red \text{ then } NT=green]$ is the same as $[NT=green \text{ then } WA=red]$

Use Breadth First Search or Depth First Search?

 
13/27

---
**Navigation**
[[L4-Slide-12|Previous ← CSP Search vs Standard Search]]
[[L4-0-Table-of-Contents|↑ Lecture 4 TOC]]
[[L4-Slide-14|Next → Backtracking Search Concept]]
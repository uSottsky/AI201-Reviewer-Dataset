# Map Coloring

![[Pasted image 20260315012414.png]]
> Reference: Slide 6 - (a) Map of Australia with territories WA, NT, SA, Q, NSW, V, T. (b) Constraint graph connecting adjacent territories.

### What is CSP?
**Task:** color each region with red, green, or blue such that no two neighboring regions have the same color.

* $X = \{WA, NT, Q, NSW, V, SA, T\}$
* $D = \{red, green, blue\}$ for each variable
* $C = \{SA \ne WA, SA \ne NT, SA \ne Q, SA \ne NSW, SA \ne V, WA \ne NT, NT \ne Q, Q \ne NSW, NSW \ne V\}$

$SA \ne WA$ is a shortcut for $\{ (SA, WA), SA \ne WA \}$
$SA \ne WA$ enumerated as $\{(red, green), (red, blue), (green, red), (green, blue), (blue, red), (blue, green)\}$

**One solution:** $\{WA=red, NT=green, Q=red, NSW=green, V=red, SA=blue, T=red\}$
Represent / visualize CSP as a constraint graph in (b).

 
6/27

---
**Navigation**
[[L4-Slide-05|Previous ← Assignments & Solutions]]
[[L4-0-Table-of-Contents|↑ Lecture 4 TOC]]
[[L4-Slide-07|Next → Example: Job-shop Scheduling (Part 1)]]
# Constraint Propagation



### Arc Consistency
$X \rightarrow Y$ is consistent if and only if 
	for every value $x$ (tail) of $X$ there is some allowed $y$ (head).


![[Pasted image 20260315014804.png]]
> Reference: Slide 21 - Visual trace continuing from Slide 20. Shows the backward propagation where neighbors of a constrained variable are rechecked and updated.


If $X$ loses a value, neighbors of $X$ need to be rechecked.

Arc consistency detects failure earlier than forward checking and can be run as a processing step after each assignment.

 
21/27

---
**Navigation**
[[L4-Slide-20|Previous ← Arc Consistency (Trace 1)]]
[[L4-0-Table-of-Contents|↑ Lecture 4 TOC]]
[[L4-Slide-22|Next → AC-3 Algorithm]]
# Constraint Propagation

![[Pasted image 20260315014737.png]]
> Reference: Slide 20 - Visual trace of Arc Consistency applied. Shows the table of domains updating and crossing out invalid colors based on arc checks.

### Arc Consistency
$X \rightarrow Y$ is consistent if and only if for every value $x$ (tail) of $X$ there is some allowed $y$ (head).

If $X$ loses a value, neighbors of $X$ need to be rechecked.

 
20/27

---
**Navigation**
[[L4-Slide-19|Previous ← Constraint Propagation: Arc Consistency]]
[[L4-0-Table-of-Contents|↑ Lecture 4 TOC]]
[[L4-Slide-21|Next → Arc Consistency (Trace 2)]]
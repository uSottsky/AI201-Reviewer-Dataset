# Forward Checking

**Forward checking:**
* propagates information from assigned to unassigned variables
* doesn't provide early detection for all failures

>![[Pasted image 20260315014449.png]]
> Reference: Slide 18 - Visual trace continuing from Slide 17. Shows a state where NT and SA both only have 'blue' left as a valid option, which is an inevitable failure.


*(From diagram)*: NT and SA cannot both be blue.

**Constraint propagation** repeatedly enforces constraints locally.

 
18/27

---
**Navigation**
[[L4-Slide-17|Previous ← Forward Checking (Trace)]]
[[L4-0-Table-of-Contents|↑ Lecture 4 TOC]]
[[L4-Slide-19|Next → Constraint Propagation: Arc Consistency]] 
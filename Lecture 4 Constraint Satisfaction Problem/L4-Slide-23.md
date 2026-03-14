# Problem Structure 


> ![[Pasted image 20260315015241.png]]
> Reference: Slide 23 - Constraint graph of Australia highlighting that Tasmania (T) is disconnected from the mainland network.

### Exploiting Problem Structure 

Mainland and Tasmania can be treated as independent subproblems. 

Subproblems are identified as Connected Components of Constraint Graph. 

Subproblem has $c$ variables out of $n$ total variables. 
$n=80$, $d=2$, $c=20$; 10 million nodes/sec 
* $2^{80}$: 4 billion years 
* $4 \cdot 2^{20}$: 0.4 seconds 

Cost (worst case): $(n/c) \cdot d^{c}$ (linear in $n$) 

 
23/27 

--- 

**Navigation**
[[L4-Slide-22|Previous ← AC-3 Algorithm]] [[L4-0-Table-of-Contents|↑ Lecture 4 TOC]] 
[[L4-Slide-24|Next → Tree-Structured CSP]]
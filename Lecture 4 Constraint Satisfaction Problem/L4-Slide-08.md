# What is CSP?

For each wheel, affix the wheel (1 min), then tighten the nuts (2 mins), and attach the hubcap (1 min).
* $Wheel_{RF} + 1 \le Nuts_{RF}; Nuts_{RF} + 2 \le Cap_{RF};$
* $Wheel_{LF} + 1 \le Nuts_{LF}; Nuts_{LF} + 2 \le Cap_{LF};$
* $Wheel_{RB} + 1 \le Nuts_{RB}; Nuts_{RB} + 2 \le Cap_{RB};$
* $Wheel_{LB} + 1 \le Nuts_{LB}; Nuts_{LB} + 2 \le Cap_{LB};$

If there are 4 workers that will install the wheels but they have to share one tool that helps put the axle in place, we need a **disjunctive constraint** to say that $Axle_{F}$ and $Axle_{B}$ must not overlap in time:
* $(Axle_{F} + 10 \le Axle_{B}) \text{ or } (Axle_{B} + 10 \le Axle_{F})$

Inspection comes last and takes 3 mins. For every variable except Inspect, we had a constraint of the form:
* $X + d_{X} \le Inspect$

**Requirement:** get the whole assembly done in 30 minutes
* $D_{i} = \{0, 1, 2, 3, ..., 30\}$

 
8/27

---
**Navigation**
[[L4-Slide-07|Previous ← Example: Job-shop Scheduling (Part 1)]]
[[L4-0-Table-of-Contents|↑ Lecture 4 TOC]]
[[L4-Slide-09|Next → Real-world CSPs]]
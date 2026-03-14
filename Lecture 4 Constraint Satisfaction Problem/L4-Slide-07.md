# What is CSP?

### Job-shop Scheduling
**Car assembly** - composed of tasks that are modeled by variables whose value is the time it takes for a task to finish.

15 tasks: install axles (front and back), affix four wheels (right, left, front, back), tighten nuts for each wheel, affix hubcaps, and inspect final assembly.

$X = \{Axle_{F}, Axle_{B}, Wheel_{RF}, Wheel_{LF}, Wheel_{RB}, Wheel_{LB}, Nuts_{RF}, Nuts_{LF}, Nuts_{RB}, Nuts_{LB}, Cap_{RF}, Cap_{LF}, Cap_{RB}, Cap_{LB}, Inspect\}$

**Precedence constraints:** task $T_{1}$ takes duration $d_{1}$ and must occur before $T_{2}$:
$T_{1} + d_{1} \le T_{2}$

Axles have to be in place before wheels and it takes 10 mins to install an axle:
* $Axle_{F} + 10 \le Wheel_{RF}; Axle_{F} + 10 \le Wheel_{LF};$
* $Axle_{B} + 10 \le Wheel_{RB}; Axle_{B} + 10 \le Wheel_{LB}$

 
7/27

---
**Navigation**
[[L4-Slide-06|Previous ← Example: Map Coloring]]
[[L4-0-Table-of-Contents|↑ Lecture 4 TOC]]
[[L4-Slide-08|Next → Example: Job-shop Scheduling (Part 2)]]
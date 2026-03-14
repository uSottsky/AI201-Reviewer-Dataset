# Alpha-Beta Pruning

* **$\alpha$**: value of the best (i.e., highest value) choice we have found so far at any choice point along the path to Max. ($\alpha = $ "at least")
* **$\beta$**: value of the best (i.e., lowest value) choice we have found so far at any choice point along the path to Min. ($\beta = $ "at most")

$\alpha-\beta$ search prunes the remaining branches at a node as soon as the value of the current node is known to be worse than the current $\alpha$ or $\beta$ value for MAX or MIN respectively.

**Alpha-Beta Pruning** - highly dependent on the order in which states are examined
* examine first successors that are likely to be best
* **perfect ordering:** $O(b^{m/2})$ instead of $O(b^m)$
* **random ordering:** $O(b^{3m/4})$

Ordering in Chess: captures, threats, forward moves, backward moves

 
17/34

---
**Navigation**
[[L3C-Slide-16|Previous ← Alpha-Beta Pruning Concept]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-18|Next → Alpha-Beta Algorithm Pseudo-code]]
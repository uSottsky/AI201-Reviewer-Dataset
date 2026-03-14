# Comparison of Blind Search Strategies 
### Comparison of Blind Search Strategies

|**Criterion**|**Breadth-First**|**Uniform-Cost**|**Depth-First**|**Depth-Limited**|**Iterative Deepening**|**Bidirectional**|
|---|---|---|---|---|---|---|
|**Complete?**|Yes|Yes|No|No|Yes|Yes|
|**Optimal cost?**|Yes|Yes|No|No|Yes|Yes|
|**Time**|$O(b^d)$|$O(b^{1+\lfloor C^*/\epsilon\rfloor})$|$O(b^m)$|$O(b^l)$|$O(b^d)$|$O(b^{d/2})$|
|**Space**|$O(b^d)$|$O(b^{1+\lfloor C^*/\epsilon\rfloor})$|$O(bm)$|$O(bl)$|$O(bd)$|$O(b^{d/2})$|


**Evaluation Caveats**:

- **b**: branching factor
- **m**: maximum depth of the search tree
- **d**: depth of the shallowest solution
- **l**: depth limit
- **Complete?**: Yes, if b is finite ; for Uniform-Cost, also requires all action costs to be $\ge \epsilon > 0$
- **Optimal cost?**: Yes, if all action costs are identical 
- **Bidirectional**: Complete and optimal if both directions are breadth-first or uniform-cost

41/41 

--- 

**Navigation** 
[[L3A-Slide-40|Previous ← Bidirectional Search Algorithm]] 
[[L3A-0-Table-of-Contents|↑ Lecture 3A TOC]]
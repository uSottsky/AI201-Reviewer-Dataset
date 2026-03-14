# Heuristic Alpha-Beta Tree Search

Performance of the chess program depends greatly on the quality of its evaluation function.
* quality = how close evaluation function value is to pay-off value
* trade-off between accuracy of evaluation function and its time cost (base-level/meta-level trade-off)
* computing material advantage is fast since the value of a piece can be judged independently of other pieces (use a weighted linear function)
* computing positional feature is time consuming (e.g. isolated pawn - requires that positions of other pawns be considered) (use a nonlinear evaluation function)

### Linear Evaluation Function
$$Eval(s) = w_1f_1(s) + w_2f_2(s) + ... + w_nf_n(s) = \sum_{i=1}^{n} w_i f_i(s)$$
* strong assumption: features are independent of each other

### Use Non-linear Evaluation Function (e.g., Neural Networks)
 
21/34

---
**Navigation**
[[L3C-Slide-20|Previous ← Evaluation Functions for Chess]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-22|Next → Cutting Off Search]]
# Heuristic Alpha-Beta Tree Search 

$$ H-Minimax(s, d) = \begin{cases} Eval(s, Max) & \text{if } IsCutoff(s, d) \\ \max_{a \in Actions(s)} H-Minimax(Result(s, a), d + 1) & \text{if } ToMove(s) = Max \\ \min_{a \in Actions(s)} H-Minimax(Result(s, a), d + 1) & \text{if } ToMove(s) = Min \end{cases} $$

* heuristic evaluation function $Eval(s,p)$ returns estimate of the expected utility of state $s$ for player $p$ 
* for terminal states: $Eval(s,p) = Utility(s,p)$ 
* for non-terminal states: $Utility(loss,p) < Eval(s,p) < Utility(win,p)$ 
* $IsTerminal(s)$ replaced with $IsCutoff(state, depth)$ 

 19/34 
 
  --- 
 
 **Navigation**
[[L3C-Slide-18|Previous ← Alpha-Beta Algorithm Pseudo-code]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-20|Next → Evaluation Functions for Chess]]
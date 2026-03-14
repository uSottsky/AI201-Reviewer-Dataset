# Heuristic Alpha-Beta Tree Search

**2. Some portions of the game tree are "hotter" than others**
* a move that leads to lengthy exchanges of pieces should be investigated with greater depth than others
* these portions are characterized by rapidly changing values of the evaluation function
	* values of evaluation function become unreliable at this point
	* use evaluation function only when its value is slowly changing from ply to ply (quiescent positions)
	
	* **Quiescence Search** - expand non-quiescent positions further until quiescent positions are reached
	
	* **Singular Extension Search** [Anantharaman et.al. 1990]
		  * a particular node should be examined further (to greater depth) if one of the opponent's moves leads to a result vastly preferable to him than all other options
		  * since this move is "forced" in some sense, the effective branching factor is small
		  * believed to be the reason why DEEPTHOUGHT outperformed its predecessor HITECH

 
24/34

---
**Navigation**
[[L3C-Slide-23|Previous ← The Horizon Effect]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-25|Next → Forward Pruning and ProbCut]]
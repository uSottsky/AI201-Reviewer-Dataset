# Heuristic functions for N-Puzzle


![[Pasted image 20260314151437.png]]

Start State
Goal State

1. $h_{1}=$ number of tiles in the wrong position
	- admissible because a tile that is out of place must be moved at least once
2. Manhattan Distance, $h_{2}=$ sum of the horizontal and vertical distances of a misplaced tile from its goal position
	-  admissible since the number of steps a tile has to move is at least equal to the sum of the horizontal and vertical distances of the misplaced tile

17/25

---
**Navigation** [[L3B-Slide-16|Previous ← Complexity]]  
[[L3B-0-Table-of-Contents|↑ Lecture 3B TOC]]  
[[L3B-Slide-18|Next → Heuristic Accuracy]]
# Search for Solutions
![[Pasted image 20260314131916.png]]
* a search tree is built during search; root of the search tree is the search node which corresponds to the initial state
* when choosing an option, we should take note of the other options so that we can backtrack in case our choice does not lead us to a solution
* choice of what state to expand next is dictated by the search strategy
* leaf nodes of a tree correspond to states that do not have successors in the tree, either because they have not been expanded yet, or because they were expanded but generated an empty set
* a search algorithm chooses one unexpanded leaf node to expand

21/41

---
**Navigation**
[[L3A-Slide-20|Previous ← Generating Action Sequences]]
[[L3A-0-Table-of-Contents|↑ Lecture 3A TOC]]
[[L3A-Slide-22|Next → Nodes vs States]]
# $F_1$ and $F_\beta$-Scores

**$F_1$-Score** - harmonic mean of the Precision and Recall
$$F_1 = 2 \cdot \frac{P \cdot R}{P+R} = \frac{TP}{TP + \frac{1}{2}(FP+FN)}$$

* provides a more sensitive measure than accuracy
* useful when:
  * there are differing costs of FP and FN (important for healthcare)
  * there is class imbalance

**$F_\beta$-Score** - allows giving more weight to Precision or Recall
$$F_\beta = (1+\beta^2) \cdot \frac{P \cdot R}{(\beta^2 \cdot P)+R} = \frac{(1+\beta^2)TP}{(1+\beta^2)TP + \beta^2 FN + FP}$$

* set $\beta=2$ if we consider Recall to be twice as important as Precision

---
**Navigation**
[[L6B-Slide-04|Previous ← Precision and Recall]]
[[L6B-0-Table-of-Contents|↑ Lecture 6B TOC]]
[[L6B-Slide-06|Next → Precision, Recall, and F1-Score Example]]
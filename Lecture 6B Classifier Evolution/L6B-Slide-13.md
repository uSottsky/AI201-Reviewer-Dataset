# Receiver Operating Characteristic (ROC)



For binary classification, there is a trade-off between high sensitivity (detect all persons who have a disease) versus high specificity (avoid false alarms, detect all persons who are healthy).
* decision threshold is applied to classifier output; value of threshold defines values of sensitivity and specificity

![[Pasted image 20260316023357.png]]
> Reference: Slide 13 - Graph of two overlapping normal distributions ("Cases without disease" and "Cases with disease") separated by a dashed vertical decision threshold. The regions TN, TP, FN, and FP are shaded.

* **decrease threshold:** FPR (Sensitivity) ↓ and FNR (Specificity) ↑
* **increase threshold:** FPR (Sensitivity) ↑ and FNR (Specificity) ↓
* for both cases the confusion matrix will have different values

---
**Navigation**
[[L6B-Slide-12|Previous ← Multiclass Confusion Matrix Example]]
[[L6B-0-Table-of-Contents|↑ Lecture 6B TOC]]
[[L6B-Slide-14|Next → ROC Curve Concept]]
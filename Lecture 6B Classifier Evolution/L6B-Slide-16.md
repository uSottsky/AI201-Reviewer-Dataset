# Matthews Correlation Coefficient

**Matthews Correlation Coefficient** - measures correlation between observed and predicted classifications
$$MCC = \frac{TP \cdot TN - FP \cdot FN}{\sqrt{(TP+FP)(TP+FN)(TN+FP)(TN+FN)}}$$

* $-1 < MCC < 1$
* high score if classifier is doing well on both negative and positive elements

**Example:** $TP=95, FP=5, TN=0, FN=0$
* does well on positive instance but unable to recognize negative elements
* $Accuracy = 91\%$
* $F_1 = 95.24\%$
* $MCC = 0.14\%$ (almost random guessing)

---
**Navigation**
[[L6B-Slide-15|Previous ← Area Under the Curve (AUC)]]
[[L6B-0-Table-of-Contents|↑ Lecture 6B TOC]]
[[L6B-Slide-17|Next → MSE and MAE]]
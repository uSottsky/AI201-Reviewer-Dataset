# Word of Caution on PPV and NPV

* PPV (NPV): if my classifier says that I have (don't have) the disease, how much should I believe it
* PPV and NPV are not only dependent on the classifier performance but also on how many cases of different classes are present in the datasets (prior probabilities)
* both are influenced by the ratio of disease and healthy cases in the test set
* both should not be used to compare classifiers' performances when those performances have been derived from different datasets (sensitivity and specificity do not have this problem)
* affected when training sets use data augmentation or artificially balanced when a certain class is underrepresented.

---
**Navigation**
[[L6B-Slide-09|Previous ← PPV and NPV]]
[[L6B-0-Table-of-Contents|↑ Lecture 6B TOC]]
[[L6B-Slide-11|Next → Balanced Accuracy]]
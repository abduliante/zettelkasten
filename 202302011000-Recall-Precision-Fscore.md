## Recall, Precision, and F score

My secret sauce to know the difference between recall and precision is the following:

* When I'm not affording to have any false negatives --> Prioritize recall.
* When I'm not affording to have any false positives --> Prioritize precision.


## F Score formula
F score is a metric that in essense (F1 score) provides a balance between precision and recall. Having different scores (F2, F0.5, F5) provide more weight to either recall or precision. The following formula is used for F beta score:

$F_{\beta } = (1+\beta ^2) \cdot \frac{Precision\cdot Recall}{(\beta^2 \cdot Precision) + Recall}$
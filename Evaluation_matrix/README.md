This folder contains th source codes for evaluation matrix.

In this study evaluation is accomplished by using the matching EO4GEO BoK concepts by the proposed NLP-based tool with the BoK Concepts by manual annotation using BAT tool given by the author for the different annotation approaches.

To measure the effectiveness of the proposed NLP tools, key performance metrics, namely precision (P%), recall (R%), and F1-score (F%), are calculated. 

The PDF document is classified using a multi-class classification method, wherein the classes correspond to the total number of EO4GEO BoK concepts within each annotation approach (952 for FULL, 346 for LEAF, and 14 for TOP). 

The evaluation employs a micro-averaging method for multi-class classification, ensuring equal weight is given to each instance across all classes. 

Micro-averaging involves aggregating the counts of true positives (TP), false positives (FP), and false negatives (FN) across all classes, subsequently computing precision and recall based on these total counts

* Total True Positive (TP) is the sum of true positive counts across all classes.
* Total False Positive (FP) is the sum of false positive counts across all classes.
* Total False Negative (FN) is the sum of false negative counts across all classes.

**Precision (P%):** a measure of the accuracy of positive predictions, is calculated by dividing the total true positives by the sum of total true positives and false positives. 
This ratio provides the proportion of correctly predicted positive instances among all instances predicted as positive 

**Recall (R%):** assesses the model's ability to capture all positive instances, is determined by dividing the total true positives by the sum of total true positives and false negatives. This ratio calculates the effectiveness of the model in identifying and correctly classifying all actual positive instances

**F1-score (R%):**  a metric commonly used in classification tasks to evaluate a model's performance, especially when there is an imbalance between the classes. It is the harmonic mean of precision and recall and provides a balanced measure that considers both false positives and false negative


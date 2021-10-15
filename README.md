# Multiclass-Classification-OvR-
implement One-versus-Rest (OvR) strategy transforming multiclass classification problems to multiple binary classification problems.
Note the difference among Seeds dataset (with 7 features and 3 classes), 2D Seeds dataset (with 2 features and
3 classes). Please use the provided training and testing set.
Please submit your code and report (including screen shot of code and the relevant figures).
1. Load the Seeds dataset.
2. Form 2 class-Seeds dataset by removing first class (Kama), compare performance of Perceptron and SVM
on testing set. Provide accuracies, confusion matrix for both model and make commnets on the
performance. (8 marks)
3. Build OvR-Perceptron and OvR-SVM and test on Seeds testing dataset (which contains 3 classes).(18 marks
for each classifier; 54 marks in total)
For each binary classifier:
Obtain the binarized labels.1 for positive class, -1 for negative class (OvR). (2 marks)
Obtain the Percepton's confusion matrix and accuracy (3 marks)
Obtain the SVM's confusion matrix and accuracy (3 marks)
Plot Perceptron's decision boundary (4 marks)
Plot SVM's decision boundary (4 marks)
Compare performance of two models and make comments for each class at the end. (2 marks)
Inputs: X, y, estimator
 yBin = binarize( y)
 build a list of estimators for each class
Output: a list of estimators
1234
Inputs: X, a list of estimators
 argmax of each estimator's confidence score on X
12
4. Use argmax to aggregate confidence scores and obtain the final label and obtain the performance (i.e.,
confusion matrix, accuracy, plotting correct and wrong prediction points) of OvR-Perceptron (5 marks) and
OvR-SVM (5 marks)
Accuracy (1 marks for each model)
Confusion Matrix (2 marks for each model)
Plotting correct and wrong prediction points (2 marks for each model)
5. Improve an alternative aggregation strategy instead of existing argmax function based OvR, using the third
5. Improve an alternative aggregation strategy instead of existing argmax function based OvR, using the third
step's results, obtain the performance (i.e., confusion matrix, accuracy, plotting correct and wrong
prediction points) of your own strategy, and explain why your strategy is better/worse than existing OvR
(20 marks)
Aggregation strategy design (10 marks)
Explanation of your own strategy (3 marks)
Confusion matrix, accuracy, plotting correct and wrong prediction points (5 marks)
Performance comparison of argmax and your own strategy (2 Marks)
6. Provide a conclusion section on your report. Include overview of what you have done and learnt during the
assignment. Aim no less than one third of a page and no more than half page. (8 Marks)
Models (Perceptron and SVM)
OvR strategy
Argmax
Aggregation Strategy etc

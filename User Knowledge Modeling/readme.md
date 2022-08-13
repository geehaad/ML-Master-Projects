<h1>Overview:</h1>
<ul>
<li> The goal of this project is to predict user knowledge by
coming up with a model based on variables to classify the
level of user knowledge.
<li> Alongside factors such as exam performance, degree of study
time and other such features, we want to explore the effect
these factors have on predicting the user knowledge level
(UNS).
</ul>

<h1>The Work:</h1>

1. Investigate the dataset:
- Visualization.
- Preprocessing.
- Encode Categoric column_ Label column: “UNS”.
2. Feature Selection:
 - Correlation Matrix
 - univariate Feature Selection or Testing applied statistical tests.
 - coef. Parameter in SVM.
3. Modeling and evaluation:
 - SVM.
 - Perceptron.
 - OVR-SVM.
 - OVO-SVM.
 
 

<h2>Conclusion:</h2>
<h4>In this project, we implemented different algorithms and technique to solve the problem
of user knowledge, we learned:</h4>
* Feature selection using: 
- Correlation Matrix, 
- univariate Feature Selection,
- .coef parameter.
* Models:
 • SVM: with linear and nonlinear, and the nonlinear kernel shows better performance
 than linear kernel, with an accuracy of 96%, 97% for training and testing, on order.
 • Perceptron: This model shows result worse than the SVM mode, with an accuracy
 of 72%, 66% for training and testing, on order.

- Approaches:
   • OvR-SVM Approach: we made four models by label one class with 1 and the rest
   with 0 for the four classes.
   • OvO-SVM Approach: For each pair of classes, we labeled one class with 0, and the
   other with 1, and came out with six classes, and in turn, models.
   we calculated the num of classes = (NumClasses*(NumClasses–1)) / 2
   
- Aggregated results:
   • OvR-SVM: After the binarization, we calculated the confidence score for these
   classes and used the argmax to get the index of the maximum value of confidence
   score.
   • OvO-SVM: We have 6 classes and got 3 confidence score for each class, so we sum
   each class confidence score, and take the mean, and used the argmax to get the index
   of the maximum value of confidence score.
- We visualized each result of our approaches.


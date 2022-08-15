<h1>Pen-Digits Classification</h1>

<h2>Modeling</h2>
<li>
Decision Tree
<li>
XGBoost

<h2>Visualization</h2>
Confusion matrix


<h2>Ensamble learning</h2>
<ul>
We create estimator using SVM and Decision Tree algorithms as base estimators,
compare their accuracies and plot the confusion matrix
<li>
Bagging
<ul>
    <li>
      SVM base estimator
    <li>
    Decision Tree base estimator
    <li>
    Majority voting
        
     We used the two estimated models(SVM, Decision tree) in majority voting algorithm.
    </ul>
    
<li>
Boosting
    
    We use Gradient Boosting classifier to classify test set samples.
    <ul>
    <li>
        First, we tune the number of estimators, we used fixed number of learning rate = .1, and
used different number of estimators [10, 50, 150, 200]
        
        <li>
            Then, we tune the learning rate, we used the best number of estimators = 200, and used
different Learning rates [.1, .3, .6, .9]

        </ul>
<li>we used XGBoost classifier with the same number of estimator
and learning rate we obtained in the previous question.
</ul>

<pr><b>Which metric is the best to compare performance, accuracy or confusion
matrix?</b>
Accuracy performance metrics can be decisive when dealing with imbalanced
data, hence, overfitting.
The confusion matrix, precision, recall, and F1 score gives better intuition of
prediction results as compared to accuracy.</pr>

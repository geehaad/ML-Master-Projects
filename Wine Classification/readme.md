<h1>Overview</h1>
We are working with two datasets: 
1. Wine dataset with Naive Bayies Classifier,
2. Car evaluation dataset with KNN.

* Visualization:
1.  Draw the Decision Boundaries,
2.  Correlation Matrix.

* Feature Selection:
1.  Correlation Matrix.

Modeling and evaluation:
1. Naive Bayies(GaussianNB)

2. KNN:
  -We use different number of training samples to show the impact of numberoftraining samples. - with 10 separate KNN classifiers and show their performance
   (Accuracy score) on the validation set and testing set
  - We tried to choose the best k values when using 100% of the training data. We trained the model with difference k values (1:10) .
  - Analysis the training time when use different number of training samples
 Conclusion:
  - After using different percentage of training samples toshowthe impact of number of training samples, we notice that there is directlyproportional relation between percentage of dateset and AccuracyofTraining, Validation and testing. But these results can vary when we run it multiple times, andits
  changes over time may lead the accuracy of 80%samples be higher than90% then decrease slightly. We conclude that in general as we increase percentage of dateset theaccuracy of the model increase, but, we should take care if this is overfitting or not by showing F1, Precision, and recall, beside the accuracyon testing and validation if still low that means there is over fittingelsemean model is good to 
  - K value indicates the count of the nearest neighbors. Updating distance metrics with every iteration is computationallyexpensive, and that’s why KNN is a lazy learning algorithm. We tried to find the best k. We conclude that as value of k increase that does not mean the accuracyof validation will increase. The best accuracy of our experiment is 89.667%with k equal 6.

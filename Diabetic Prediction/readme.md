<h1>Overview</h1>
We work with Diabetic dataset; the dataset contains 576 rows and 8 columns.

<h1>Classifiers:</h1> 
• We used 2 classifiers: 
  <ul>
  <li><b>LR</b>,
  and <li> <b>K-NN</b>
 
classifiers on our dataset, and 
<li>  We plot the TSNE for each classifier, one for training and another for testing 
data. 
 </ul>
<h1> K-means Clustering algorithm </h1>
• We also use K-means algorithm to cluster our data, choose the best number of clusters using the silhouette score.

<h1>Dimensionality Reduction (DR)</h1>
- We Apply PCA on LR and K-NN classifiers to find the best number of features.
- For each algorithm (LR and KNN) we tried various number of PCA components and checked the test accuracy for each one.

<h1>Feature Selection methods :</h1>
<ul>
  <li>
• Information gain
   <li>
• Wrapper method
 </ul>
- We use <b>Information gain</b> in Filter method and forward Elimination in 
Wrapper methods.
<br>
- In <b>wrapper method</b> we use forward elimination and train KNN and logistic 
regression started from 1 best selected feature to all features and see best accuracy 
based on best selected features.

<h1>SOM</h1>
<pr>An SOM is mainly used for data visualization and provides a quick visual 
summary of the training instances. In a 2D rectangular grid, each cell is 
represented by a weight vector. 
  
For a trained SOM, each cell weight 
represents a summary of a few training examples.

Cells in the close vicinity of 
each other have similar weights, and like examples can be mapped to cells in 
a small neighborhood of each other.</pr>

• We initialize number of neurons with 2 and iterate to 30 neurons ,train SOM algorithm with 
each number of neuron and plot silhouette score for each number of neurons algorithm train 
on then plot initial and final position of neurons.

<h1>DBSCAN</h1>
<b>Density-Based</b> Spatial Clustering of Applications with
Noise (DBSCAN) is a base algorithm for density-based clustering, It can 
discover clusters of different shapes and sizes from a large amount of data, 
which is containing noise and outliers.<br>

DBSCAN does not require one to specify the number of clusters in the 
data a priori, as opposed to k-means.<br>

<h3>The DBSCAN algorithm uses two parameters:</h3><br>
• minPts: The minimum number of points clustered together for a 
region to be considered dense.<br>
• eps (ε): A distance measure that will be used to locate the points 
about any point.<br>
<h4>In this point we tune the hyperparameters:</h4>
- Epsilon (0.3 : 0.70)<br>
- Minppoints (2 : 15)<br>
We tried each combination of Epsilon and min-point and produce its 
Silhouette score



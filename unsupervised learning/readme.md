## Application:

### 1. K-Means Clustering:
KMeans clustering algorithm works by first determining centroids of the clusters and second assigning instances to the clusters and the whole process is repeated until convergence.
   1. Unsupervised preprocessing followed by classification:  
   The goal is to improve classification performance. Unsupervised preprocessing using K-Means is followed by Logistic Regression classification. Clustering improves accuracy from 96.89% to 98%.
   2. Semi-Supervised Learning with K-Means:     
   Semi-Supervised Learning is a combination of unsupervised and supervised algorithms using a dataset that is partially labeled.  
   Given a partially labeled dataset, clustering may be an effective way to label the dataset automatically.  
   KMeans algorithm applied to the digits dataset achieves an accuracy rate of about 93.8% compared to the baseline of 96.9%.
   3. Limit of K-Means:  
   Nonspherical shapes are not captured properly.

### 2. Gaussian Mixture Model Anomaly_Detection:
Gaussian Mixture Model is used for anomaly detection. 
Instances located in low-density regions will be detected as anomalies.

### 3. Variational Bayesian Gaussian Mixtures:
Automatically searching for the optimal number of clusters.
Set the number of components to a value greater than the optimal number of clusters, 
and the algorithm will eliminate the unnecessary clusters automatically.

Test the model on a dataset with 2 moon-shaped clusters.
Instead of detecting 2 moon-shaped clusters, the algorithm detected 8 ellipsoidal clusters. 
However, it may be an acceptable solution for anomaly detection.
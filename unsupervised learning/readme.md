## Application:

### 1. K-Mean:

   1. Preprocessing:  
   Using K-Means algorithm to improve classification performance. Unsupervised preprocessing using K-Means is followed by Logistic Regression classification.

   2. Semi-Supervised Learning with KMeans:
   Semi-Supervised Learning: combination of unsupervised and supervised algorithms using a dataset that is partially labeled.

### 2. Gaussian_Mixture_Model_Anomaly_Detection:
Gaussian Mixture Model is used for anomaly detection. 
Instances located in low-density regions will be detected as anomalies.

### 3. Variational_Bayesian_Gaussian_Mixtures:
Automatically searching for the optimal number of clusters.
Set the number of components to a value greater than the optimal number of clusters, 
and the algorithm will eliminate the unnecessary clusters automatically.

Test the model on a dataset with 2 moon-shaped clusters.
Instead of detecting 2 moon-shaped clusters, the algorithm detected 8 ellipsoidal clusters. 
However, it may be an acceptable solution for anomaly detection.
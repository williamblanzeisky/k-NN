# K-Nearest Neighbors (KNN)

The KNN algorithm is a robust and versatile classifier that is often used as a benchmark for more complex classifiers such as Artificial Neural Networks (ANN) and Support Vector Machines (SVM). Despite its simplicity, KNN can outperform more powerful classifiers and is used in a variety of applications such as economic forecasting, data compression and genetics.

KNN Algorithm is in the categegory of unsupervised learning, with the charateristics of non-parametric and instance-based. KNN does not explicitly learn from the training data but instead, it memorizes the training data for future prediction (which is why KNN is lazy). The way KNN works is that it finds K-nearest points to the query point. The nearest point can be calculated using distance metrics, such as Euclidean distance (L2-Norm), Manhattan distance (L1-Norm) etc. For classification, the query point will use the majority votes class. For regression, the predicted y value could be the average or median of the nearest neighbors.

The limitation of KNN is that the time and space complexity can be large, approximately O(N*D). KNN can also suffer from skewed distribution of classes (since it is using the majority vote). To overcome this limitation, weighted-KNN is introduced. Weighted KNN gives more weight to points that are closer to the query point. This point can be the inverse of the distance between query point to the nearest neighbors. In addition, to reduce the time complexity of KNN, other implementation using KD-Tree and LSH using cosine similarity/euclidean distance is used.

Files included:
1. KNN - Decision Boundary: created function to plot decision boundary using pcolormesh and np.meshgrid
2. KNN - MLXTEND: using MLXTEND to plot decision regions
3. KNN - CrossVal: use k-fold cross validation method to find K
4. KNN - RandomSearchCV: Implement RandomSearchCV with k fold cross validation on KNN from scratch
5. KNN - GridSearchCV: Implement GridSearchCV with k fold cross validation on KNN from scratch

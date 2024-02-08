# PREDICTION OF POTENTIALLY HAZARDOUS ASTEROIDS
The problem statement is to develop an ML
model to classify hazardous asteroids. It
helps to easily identify and track asteroids
which are hazardous and allow timely risk
management.
The Approach aims at outlining subgroups
of near earth asteroids (NEAs) with high
PHA concentration in them.

# OVERVIEW OF THE WORKFLOW:
1.Collect the data from relevant sources

2.Do the Data Preprocesssing

3.Find the PHAs from the real data

4.Make more data using virtual asteroids

5.Choose the ML Model which will give
maximum accuracy

<!-- # Data Collection
We have collected data from the sources given
below :

https://www.kaggle.com/datasets/shrutimehta/nasa-
asteroids-classification

https://www.kaggle.com/datasets/sakhawat18/aster
oid-dataset -->

# VIRTUAL ASTEROIDS
We synthetically increase amount of data by generating virtual
asteroids and computing MOID for them. We do this inorder to
unlock more deeper insights about our data for asteroids.

Uniform Dataset : We generate new dataset assuming the various
oarameters follow uniform distribution. We do this so that we are able to
create a uniform space in ‘w’ and ‘q’ so that clustering algorithm can work
efficiently.

Non-Uniform Dataset : These are distributions that approximate
distributions of real NEAs.

# Clustering using DBSCAN
1.Ability to Find Arbitrary-Shaped Clusters: DBSCAN can detect clusters of various shapes, making it suitable for
datasets with non-uniformly shaped clusters, unlike some other algorithms like K-Means, which assume spherical
clusters.

2.Robust to Noise: It's capable of distinguishing noisy data points as outliers or noise, ensuring that they don't disrupt the
cluster formation. This makes it more robust in the presence of data imperfections.

3. No Need to Specify the Number of Clusters: Unlike K-Means,
which requires you to specify the number of clusters beforehand,
DBSCAN automatically identifies the number of clusters within the
data.

4. Efficiency: DBSCAN efficiently handles large datasets and is less
sensitive to the order of data points, which can be an issue with
hierarchical clustering.


# Results
- We used SVM, Random Forest and XG Boost model for classification in all the domains and below are the best results

## Domain 1 

## Domain 2
- Highest accuracy of classification of hazardous and non hazardous asteroid in Atiras and Atens is using XG Boost Model i.e 85.91%
- Highest accuracy of classification of hazardous and non hazardous asteroid in Apollo is using XG Boost Model i.e 94.61%
## Domain 3
- Highest accuracy of classification of hazardous and non hazardous asteroid in Apollo group is achieved using XG Boost Model i.e 94.69%

# REFERENCES
1.Prediction of Orbital Parameters for Undiscovered Potentially Hazardous
Asteroids by Vadym Pasko

2.Hazardous Asteroid Classification through Various Machine Learning
Techniques by Anish Si

3.https://github.com/nomad-vagabond/asterion?search=1


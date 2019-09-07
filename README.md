# Fuzzy-Vector-Quantization
A novel approach for Fuzzy Vector Quantization technique for pattern classification.

The classifier employs Majority Voter Circuit principles to identify the individual membership level of the fuzzified features, and thus constructs a concatenated fuzzy quantized vector as the class centroid for a given class.

The class-centroids are preserved to subsequently determine the class of an unknown pattern. 

The features of the unknown pattern are first fuzzified like the one done during the training phase, and the fuzzified features are concatenated to get a fuzzy description of the unknown data point. This data point is then projected along the unit vectors of all class centroids. The unknown data point is considered to fall in class k, if the projection along the k-th unit class centroid vector is the largest. 

The calibration of the MFs for optimal performance of the classifier is an interesting open-ended problem. Here, the MFs are selected from user’s own experience. However, for the best performance, the choice of levels and MFs of the levels may be obtained in the settings of an optimization problem. Any traditional or new meta-heuristic algorithm may be invoked to handle the present optimization problem, where a fitnees/objective function needs to be designed to maximize the classification accuracy for all the classes.

# Membership function used:
Gaussian membership function.

# Quantizer step size optimization:
The step size of the quantizer has been optimized by taking that step size when the seperation between the clusters have been found maximum. For this a list consisting of all the step size and the corresponding seperation between the class centroids has been prepared first.

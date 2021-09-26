## K-nearest neighbors 
https://github.com/scsanjay/ml_from_scratch/blob/main/02.%20K%20Nearest%20Neighbor%20(KNN)/Knn.ipynb

k-nearest neighbors aka knn is a classification technique which looks
at it's neighbors to predict label for a query point.

  Parameters
  ----------
    n_neighbors : int, default=5
        Number of nearest neighbors to look at for predicting.

    weights : {'uniform', 'distance'}, default='uniform'
        uniform gives equal importance to each neighbors.
        distance gives more importance to closer neighbor, importance = 1/distance.

    p : int, default=2
        It is parameter for the minkowski distance (lp distance). It is used only
        when metric=minkowski.

    metric : {'minkowski', 'manhattan', 'euclidean'}, default='minkowski'
        The distance metric used to check for neighbors. The default is minkowski
        with p=2 which is equivalent to euclidean.

  Attributes
  ----------
    classes_ : array of shape (n_classes,)
        It returns the class labels based on fitted data.

    n_classes_ : int
        It returns the number of distinct class labels based on fitted data.

    n_samples_fit_ : int
        It gives number of train data fitted.
        
  Methods
  -------
  
  ### fit
  Fit the training data to the model.

    Parameters
    ----------
    X : array-like of shape (n_samples, n_features)
        The training data.

    y : array-like of shape (n_samples,)
        The target labels.

    Returns
    -------
    self
 ### predict
 Predict the labels of test data.

    Parameters
    ----------
    X : array-like of shape (n_queries, n_features)
        The testing data.

    Returns
    -------
    y : array-like of shape (n_queries,)
        The target labels of test data.
        
  ### kneighbors
  Return the distances and the k nearest neighbors indices.

    Parameters
    ----------
    X : array-like of shape (n_queries, n_features)
        The testing data.

    Returns
    -------
    (distance, neighbors) : tuple of array-like of shape (n_queries, k) each
        distance is the distance of each point from the query points.
        neighbors is represents the indices of neighbors in train data.

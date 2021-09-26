## K-Nearest Neighbors regression 
k-nearest neighbors regression looks at it's neighbors to predict 
  output for a query point.

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
        The target outputs.

    Returns
    -------
    self
  
  ### predict 
  Predict the outputs of test data.

    Parameters
    ----------
    X : array-like of shape (n_queries, n_features)
        The testing data.

    Returns
    -------
    y : array-like of shape (n_queries,)
        The target outputs of test data.
      
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

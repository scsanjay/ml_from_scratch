# DBSCAN

https://github.com/scsanjay/ml_from_scratch/blob/main/10.%20Density-Based%20Spatial%20Clustering%20of%20Applications%20with%20Noise%20(DBSCAN)/DBSCAN.ipynb

DBSCAN (Density-Based Spatial Clustering of Applications with Noise) Implementation

  Parameters
  ----------
    eps : float, default=0.5
        The radius to consider.

    min_samples : int, default=5
        Minimum number of samples for a dense region.

    metric : {'minkowski', 'manhattan', 'euclidean'}, default = minkowski
        Distance measure to be used.

    p : int, default=2
        It is parameter for the minkowski distance (lp distance). It is used only
        when metric=minkowski.

  Attributes
  ----------
    labels_ : array of size n_samples
        Cluster labels of each data point. -1 if it's a noisy point.

  Methods
  -------
  
  ### fit
  It will find the clusters.

    Parameters
    ----------
    X : array of shape (n_samples, n_features)

    Returns
    -------
    self : object
    
   ### fit_predict
   It will find the clusters and return labels.

    Parameters
    ----------
    X : array of shape (n_samples, n_features)

    Returns
    -------
    labels : array of shape (n_samples,)
        Cluster labels of each data point. -1 if it's a noisy point.

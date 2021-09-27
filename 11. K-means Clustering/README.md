# Custom implementation of KMeans

https://github.com/scsanjay/ml_from_scratch/blob/main/11.%20K-means%20Clustering/KMeans.ipynb

KMeans clustering with Lloyds algorithm.

  Parameters
  ----------
    n_clusters : int, default=8
        The number of cluster to make.

    init : {'k-means++', 'random'}, default='k-means++'
        Initilisation of initial clusters.

    max_iter : int, default=300
        Maximum number of iterations.

    tol : float, default=1e-4
         Tolerance to declare convergence with Frobenius norm
         of the difference in the cluster centers of two consecutive iterations.

  Attributes
  ----------
    labels_ : array of size n_samples
        Cluster labels of each data point.
      
  Methods
  -------
  
  ### fit 
  It will find the specified number of clusters.

    Parameters
    ----------
    X : array of shape (n_samples, n_features)

    Returns
    -------
    self : object
    
  ### fit_predict
  It will find the specified number of clusters and return the labels.

    Parameters
    ----------
    X : array of shape (n_samples, n_features)

    Returns
    -------
    labels : array of shape (n_samples,)
        Cluster labels of each data point.

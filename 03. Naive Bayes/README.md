## Multinomial Naive Bayes
https://github.com/scsanjay/ml_from_scratch/blob/main/03.%20Naive%20Bayes/MultinomialNaiveBayes.ipynb

  Parameters
  ----------
    alpha : float, default=1.0

    fit_prior : bool, default=True

    class_prior : array-like of shape (n_classes,), default=None

  Attributes
  ----------
    class_count_ : ndarray of shape (n_classes,)

    class_log_prior_ : ndarray of shape (n_classes, )

    classes_ : ndarray of shape (n_classes,)

    n_classes_ : int

    feature_count_ : ndarray of shape (n_classes, n_features)

    feature_log_prob_ : ndarray of shape (n_classes, n_features)

    n_features_ : int
    
   Methods
   -------
   
   ### fit 
    Parameters
    ----------
    X : array-like of shape (n_samples, n_features)
    y : array-like of shape (n_samples,)

    Returns
    -------
    self : object
      
  ### predict
    Parameters
    ----------
    X : array-like of shape (n_samples, n_features)

    Returns
    -------
    C : ndarray of shape (n_samples,)

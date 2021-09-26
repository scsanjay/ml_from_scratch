## Decision Tree Regression with MSE.

  Parameters
  ----------
    max_depth : int, default=None
      Maximum depth that the tree can have. If None then tree grows till node
      have samples less than min_samples_split or MSE becomes 0.

    min_samples_split : int, default = 2
      Minimum number of samples required in the node to be considered
      for next split.
    
  Methods
  -------
  
  ### fit
  It will create the decision tree based on train data

    Parameters
    ----------
    X_train : array of shape (n_samples, n_features)

    Y_train : array of shape (n_samples)

    Returns
    -------
    self : object
    
  ### predict
   It will predict the output for the test data.

    Parameters
    ----------
    X_test : array of shape (n_samples, n_features)

    Returns
    -------
    predictions : array of shape (n_samples,)

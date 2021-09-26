  ## Decision Tree Classification with Gini Impurity.

  Parameters
  ----------
    max_depth : int, default=None
      Maximum depth that the tree can have. If None then tree grows till node
      have samples less than min_samples_split or gini impurity becomes 0 
      that means pure node.

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
  It will predict the output classes for the test data.

    Parameters
    ----------
    X_test : array of shape (n_samples, n_features)

    Returns
    -------
    predictions : array of shape (n_samples,)  

  ## SGD implementation of Logistic Regression
  https://github.com/scsanjay/ml_from_scratch/blob/main/05.%20Logistic%20Regression/LogisticRegression.ipynb

  Parameters
  ----------
    penalty : {'l1', 'l2'}, default l2

    alpha : float, default = 0.0001
      multiplier for the regularisation term

    eta0 : float, default = 0.0
      initial learning rate

    epoch : int, default = 1000

  Attributes
  ----------
    weights : array of size n_features

    bias : float
  
  Methods
  -------
  
  ### fit
   It will find a hyperplane that best separate the data.

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
    predicted : array of shape (n_samples,)
   

 ## SGD implementation of Support Vector Machine
 
https://github.com/scsanjay/ml_from_scratch/blob/main/06.%20Support%20Vector%20Machine/SVM.ipynb

  Parameters
  ----------
    C : float, default = 1
      Regularization parameter

    alpha : float, default = 0.0001
      Learning rate

    epoch : int, default = 1000

  Attributes
  ----------
    weights : array of size n_features
  
  Methods
  -------
  
  ### fit
  It will find the margin maximising hyperplane that best separate the data.

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

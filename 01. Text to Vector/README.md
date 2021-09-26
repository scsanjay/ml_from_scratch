## Converts a corpus into vector representation
https://github.com/scsanjay/ml_from_scratch/blob/main/01.%20Text%20to%20Vector/Bow.ipynb

Parameters
----------
    binary : bool, default=False
        If True it will return Boolean BoW.

Attributes
----------
    vocabulary_ : dict
        Dictionary with key as the features and the values as the

Methods
-------

### fit
  It will learn the vocabulary from the given corpus.

    Parameters
    ----------
    corpus : iterable
        A list of documents.

    Returns
    -------
    self
   
### transform 
  It will transform the corpus into sparsed matrix and return it.

    Parameters
    ----------
    corpus : iterable
        A list of documents.

    Returns
    -------
    scipy.sparse.csr_matrix
    
### fit_transform
  It will learn the vocabulary and transform the corpus into sparsed matrix and return it.

    Parameters
    ----------
    corpus : iterable
        A list of documents.

    Returns
    -------
    scipy.sparse.csr_matrix

### get_feature_names
  It will return the features/vocab.

    Returns
    -------
    list

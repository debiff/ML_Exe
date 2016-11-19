# ML_Exe
Machine learning exercise from udacity course

## Ex 1
In this exercise we learn how to make a naive bayes decision boundary in Python

### Step 1 - getting start with sk-learn
First of all being good learner we start reading the documentation at this link:
*[Sk-learn naive bayes] (http://scikit-learn.org/stable/modules/naive_bayes.html) includes the Gaussian Naive Bayes use case that is what we are going to be using
*[GaussianNB] (http://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.GaussianNB.html) The page of the module that we'll use

### See the first example of Gaussian Naive Bayes
We focus on the first example:
'''
>>> import numpy as np
>>> X = np.array([[-1, -1], [-2, -1], [-3, -2], [1, 1], [2, 1], [3, 2]])
>>> Y = np.array([1, 1, 1, 2, 2, 2])
>>> from sklearn.naive_bayes import GaussianNB
>>> clf = GaussianNB()
>>> clf.fit(X, Y)
GaussianNB(priors=None)
>>> print(clf.predict([[-0.8, -1]]))
[1]
'''


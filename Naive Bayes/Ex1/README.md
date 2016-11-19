In this exercise we explore the sk-learn library and test the first example

### Step 1 - getting start with sk-learn
First of all being good learner we start reading the documentation at this link:
*[Sk-learn naive bayes] (http://scikit-learn.org/stable/modules/naive_bayes.html) includes the Gaussian Naive Bayes use case that is what we are going to be using
*[GaussianNB] (http://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.GaussianNB.html) The page of the module that we'll use

### See the first example of Gaussian Naive Bayes
We focus on the first example:
```
>>> import numpy as np
>>> X = np.array([[-1, -1], [-2, -1], [-3, -2], [1, 1], [2, 1], [3, 2]])
>>> Y = np.array([1, 1, 1, 2, 2, 2])
>>> from sklearn.naive_bayes import GaussianNB
>>> clf = GaussianNB()
>>> clf.fit(X, Y)
>>> print(clf.predict([[-0.8, -1]]))
[1]
```
* the first three lines as the task of creating some training point that we can use 
* in the fourth line we import the GaussianNb module from the file naive_bayes
* in the fifth line we create the classifier, so we instatiate the GaussianNb class
* in the sixth line we fit our classifier (fit it is the same of train it), so this is where we actually give it the training data and it learns the patterns. We pass it the variable 'X' that in this case are the features, and the variable 'Y' that are the labels.
* in the last line we ask the classifier that we've just trained for some predictions, passing it a new point and obtaining a label



Based on Ex2 we must print the value of the accuracy. Accuracy is defined as the number of test points that are classified correctly divided by the total number of test points but there is also a method from sklearn

### Find a method to calculate the accuracy.
We use the same two files of Ex2, class_vis.py and perp_terrain_data.py while the file studentCode.py is new but is already complete.

### classify.py
This file is presentend as follow
```
def NBAccuracy(features_train, labels_train, features_test, labels_test):
    """ compute the accuracy of your Naive Bayes classifier """
    ### import the sklearn module for GaussianNB
    from sklearn.naive_bayes import GaussianNB

    ### create classifier
    clf = #TODO
    ### fit the classifier on the training features and labels
    #TODO
    ### use the trained classifier to predict labels for the test features
    pred = #TODO
    ### calculate and return the accuracy on the test data
    ### this is slightly different than the example, 
    ### where we just print the accuracy
    ### you might need to import an sklearn module
    accuracy = #TODO
    return accuracy
```
and in addition to the notions learned in the Ex2 we must find a method to compute the accuracy.
My solution is the following:
```
	def NBAccuracy(features_train, labels_train, features_test, labels_test):
    ### import the sklearn module for GaussianNB
    from sklearn.naive_bayes import GaussianNB
    import numpy as np
    from sklearn.metrics import accuracy_score
    ### create classifier
    clf = GaussianNB()
    ### fit the classifier on the training features and labels
    clf.fit(features_train, labels_train)
    ### use the trained classifier to predict labels for the test features
    pred = clf.predict(features_test)
    return accuracy_score(labels_test, pred, normalize=True)
```
I used the accuracy_score function that as input need the labels predicted and the true labels. The last parameter is normalize and if is true the function return the fraction of correctly classified samples otherwise return the number of correctly classified samples.

The correct result is 0.884 and if you want test it you can print the result of the NBAccuracy function
 


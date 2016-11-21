In this exercise we use the GaussianNB to train a classifier and classify a new speed regarding the grade/bumpy problem

### Complete the code in ClassifyNB.py with with the sklearn Naive Bayes classifier to classify the terrain data.
We obtain from the teacher the 3 files studentMain.py, class_vis.py, prep_terrain_data.py that in order have the task of:

*put togheter all the classes and the functions of the other files, is the entry point of our program
*is the class needed for plot graph and points
*is the file that create a dataset

### ClassifyNB.py
This file is presentend as follow
```
def classify(features_train, labels_train):   
    ### import the sklearn module for GaussianNB
    ### create classifier
    ### fit the classifier on the training features and labels
    ### return the fit classifier
    
    
    ### your code goes here!
    
```
and we have to apply the notions learned in the Ex1 for create and fit the classifier

So I changed the classify function as follow
```
def classify(features_train, labels_train):   
    ### import the sklearn module for GaussianNB
    from sklearn.naive_bayes import GaussianNB
    ### create classifier
    clf = GaussianNB()
    ### fit the classifier on the training features and labels
    clf.fit(features_train, labels_train)
    ### return the fit classifier
    return clf
```

And after the execution of studentMain.py I received the following output   

![alt tag] (https://github.com/debiff/ML_Exe/raw/master/Naive%20Bayes/Ex2/test.png)

That was the desidered output of the exercise
 


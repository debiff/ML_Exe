ud120-projects
==============

Here I develop all the code regarding the mini-project

# 1° - NB mini-project
## naive_bayes/nb_author_id.py

For that concern the first mini-project we, as in the exercises done previously, have declear a classifier, fit it and after the prediction calculate the accuracy.

The code I added is:

```python
clf = GaussianNB()

t0 = time()
clf.fit(features_train, labels_train)
print "training time:", round(time()-t0, 3), "s"

t1 = time()
pred = clf.predict(features_test)
print "training time:", round(time()-t1, 3), "s"

print "The accuracy is:" + str(accuracy_score(labels_test, pred, normalize=True))
```
The code around __clf.fit(features_train, labels_train)__ and __pred = clf.predict(features_test)__ is not necessary but I put it for know how long the training time and the prediction time are


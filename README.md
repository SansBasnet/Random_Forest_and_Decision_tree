# ML: Decision Tree Learning and Random Forest & Bagging. 

# Decision Tree  

Decision tree learning is a predictive modelling and primitive supervised machine learning techniues. The decision tree starts from observation (sunny or rainy) to conclusion about the item's target value (represented in leaves.) A tree models where target variable can take a discrete value are classification trees - leaves represent class labels and branches conjuctions of features. Decision trees where the target variable can take continuous values are called regression trees. In this repo are implementation of both trees on two different datasets. 


<br>
<p align="center">
<img src = "images/Decision tree.png"  width = "480" height = "310">
 </p>
<br>

Decision tree learning algorithm is applied on Pima diabetes and win quality datasets. 
On the 'code' folder are two python scripts that implements a basic decision tree from Scikit to make predictions. 

(1) uses dataset from Pima Indians diabetes for classification. target variable: the presence/absense of diabetes in individuals and 

(2) uses dataset from the quality of red wines rated 1-10 for regression. 

This code explores several ways to score the predictions and evalute results, including but not limited to different scorers, cross comparing cross-validation to simple test and train sets, as well as looking at the effects of simple feature selection. 

In classification, an object 'clf' is created and for regression 'rgr'. Methods such as fitting a model to some data are called on using these objects, and access their internal variables such as getting predicted class labels.


</br>

# Random Forest and Bagging 

## How does random forests work?

When the training set for the current tree is drawn by sampling with replacement, about one-third of the cases are left out of the sample. This oob (out-of-bag) data is used to get a running unbiased estimate of the classification error as trees are added to the forest. It is also used to get estimates of variable importance.

After each tree is built, all of the data are run down the tree, and proximities are computed for each pair of cases. If two cases occupy the same terminal node, their proximity is increased by one. At the end of the run, the proximities are normalized by dividing by the number of trees. Proximities are used in replacing missing data, locating outliers, and producing illuminating low-dimensional views of the data.

Features of Random Forest: 

- It is unexcelled in accuraccy among current algorithms 
- It runs efficiently on large data bases.
- It can handle thousands of input variables without variable deletion.
- It gives estimates of what variables are important in the classification.
- It generates an internal unbiased estimate of the generalization error as the forest building progresses.
- It has an effective method for estimating missing data and maintains accuracy when a large proportion of the data are missing.
- It has methods for balancing error in class population unbalanced data sets.
- Generated forests can be saved for future use on other data.
- Prototypes are computed that give information about the relation between the variables and the classification.
- It computes proximities between pairs of cases that can be used in clustering, locating outliers, or (by scaling) give interesting views of the data.
- The capabilities of the above can be extended to unlabeled data, leading to unsupervised clustering, data views and outlier detection.
- It offers an experimental method for detecting variable interactions.

</br> 

Review these Scikit API links for more information on how they are implemented. 

SVM Classifier: https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html

SVM Regressor: https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVR.html

LDA Classifier: https://scikitlearn.org/stable/modules/generated/sklearn.discriminant_analysis.LinearDiscriminantAnalysis.html

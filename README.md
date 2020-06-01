# Machine Learning: Decision Tree Learning and Random Forest. 

Decision tree learning is a predictive modelling and primitive supervised machine learning techniues. The decision tree starts from observation (sunny or rainy) to conclusion about the item's target value (represented in leaves.) A tree models where target variable can take a discrete value are classification trees - leaves represent class labels and branches conjuctions of features. Decision trees where the target variable can take continuous values are called regression trees. In this repo are implementatio of both trees on two different datasets. 



<br>
<p align="center">
<img src = "images/Decision tree.png"  width = "480" height = "310">
 </p>
<br>

Machine Learning decision tree learning algorithm is applied on Pima diabetes and win quality datasets. 
On the 'code' folder are two python scripts that implements a basic decision tree from Scikit to make predictions. 

(1) uses dataset from Pima Indians diabetes for classification. target variable: the presence/absense of diabetes in individuals and 

(2) uses dataset from the quality of red wines rated 1-10 for regression. 

This code explores several ways to score the predictions and evalute results, including but not limited to different scorers, cross comparing cross-validation to simple test and train sets, as well as looking at the effects of simple feature selection. 

In classification, an object 'clf' is created and for regression 'rgr'. Methods such as fitting a model to some data are called on using these objects, and access their internal variables such as getting predicted class labels.

Review these Scikit API links for more information on how they are implemented. 

SVM Classifier: https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html

SVM Regressor: https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVR.html

LDA Classifier: https://scikitlearn.org/stable/modules/generated/sklearn.discriminant_analysis.LinearDiscriminantAnalysis.html

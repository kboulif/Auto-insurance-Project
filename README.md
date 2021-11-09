# Auto-insurance-Project


In this project, we will explore and analyze and model a data that countains about 8000 rows. 
The target variable is 'TARGET_FLAG' which is a categorical variable that has two possible values '0' or '1'. '1' Means that 
the person was in a car crash, and '0' means that the person was not in a car crash. 
This is a classification problem that aims to predict if a person will crash its car or not. 

After EDA and preprocessing data, I trained many classifications model with and then without using PCA. The models that have been used are:
Logistic Regression, Support Vector Classifier, Decision Tree, Random Forest, Gaussian Naive Bayes, XGBOOST and AdaBoost. 

Concerning the metric, I choose the F1-score. Because at the same time, I am interested in having a good recall and precision. Indeed, I want to predict high number of car crashes among actual car crashes (this is the recall), and then when I predict that a person will 
have a car crash, I want to be right (this is the precision).

For Decision Tree Classifier and Ada Boost Classifier classifiers, I used Grid-search to find the optimal hyperparameters.  The PCA didn't improve our classifiers' performance, which could be explained by the fact that pca does not catch non-linearities between features. 
                                                                     
The model AdaBoost gives the highest score. I used it for test data. 

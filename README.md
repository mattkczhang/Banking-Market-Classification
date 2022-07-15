# Banking Market Classification

The Banking Market Classification project is a in-class group project at the University of Chicago Python for Analytics course in 2022 Spring. 

![image](https://user-images.githubusercontent.com/94136772/178913113-f146c9d2-2a3d-47f1-a8b9-aeced7014599.png)

## About the dataset

The bank dataset of different customers data is related with direct marketing campaigns (phone calls) of a Portuguese banking institution. Banking Dataset of different customers to predict if they will convert or not. The classification goal is to predict if the client will subscribe (yes/no) a term deposit (variable y).

This dataset is publicly available for research. It has been picked up from the UCI Machine Learning with random sampling and a few additional columns.

S. Moro, P. Cortez and P. Rita. A Data-Driven Approach to Predict the Success of Bank Telemarketing. Decision Support Systems, Elsevier, 62:22-31, June 2014

## Description

Term deposits are a major source of income for a bank. A term deposit is a cash investment held at a financial institution. The bank has various outreach plans to sell term deposits to their customers such as email marketing, advertisements, telephonic marketing, and digital marketing. Telephonic marketing campaigns still remain one of the most effective way to reach out to people. However, they require huge investment as large call centers are hired to actually execute these campaigns.

Therefore, this project intends to identify the customers most likely to convert beforehand so that they can be specifically targeted via call. In short, the classification goal is to predict if the client will subscribe to a term deposit (variable y) based on features like age and education level.   

The project plan can be described as following:

* We first transform, scale, and ecnode the dataset to prepare for modeling. 
* We then conduct feature engineering and exploratory data analysis to visualize the feature correlation and select the most important features.
* We prepare the training and testing set to explore unsupervised models like KNN and supervised models like logistic regression, decision tree, and random forest. 
* The results of each model are presented based on evaluation metrics including accuracy,	K-fold Accuracy, ROC,	Presion Score, and Recall Score.

## Result

<img width="1096" alt="image" src="https://user-images.githubusercontent.com/94136772/179088843-8ed7364b-55b5-4cf1-8c93-9a414cab665d.png">

* While performance of Logsitc and Random Forest are similarly good, we choose Logistic model as it has higher precision score. This is because we need a higher preicison score to maximize the return of term deposit marketing. In other words, we care more about the accuracy among the people that are modeled to be our target customers. 

* Logistic model is easy to implement and interpret and makes no assumptions about distributions of classes in feature space.
With similar accuracy and cross-validated accuracy, the Logistic model result tends to be robust.

## Limitation

* From the EDA, we know that most of the observations don’t subscribe to the term deposit. Such unbalanced dataset might lead to biased modeling and rpediction.

* We can also try ensemble method that combines the good models together like the Logistic and Random Forest model. 

* The number of observation is 4118. Although it might be large enoguh for a simple project/prediciton, it is far from enoguh to make an accurate real-world prediction.

* We can also try more advanced / black box models like neural network to achieve better accuracy at the expense of interpretability. 

## Authors

Kaichong (Matt) Zhang: University of Chicago student

Flora Huang: iversity of Chicago student

Jiawei Yu: iversity of Chicago student

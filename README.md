# Credit_Risk_Analysis

## Project Objectives: to examine different algorithms to predict credit card risk. 

## Dataset: 
https://help.lendingclub.com/hc/en-us/articles/215488038-What-do-the-different-Note-statuses-mean-

## Results: 
The images below display the classification reports for each algorithm. 

1. Random Oversampling: 

![ROS_classification report](https://user-images.githubusercontent.com/113721712/230809921-500880e4-f626-457c-b2d9-f7510dc05815.png)

Random oversampling produced an accurancy score of 66%. 

2. SMOTE Oversampling: 

![SMOTE_Classification Report](https://user-images.githubusercontent.com/113721712/230809982-ed9e2c6e-055c-4b07-9ca1-89ef1f8ac368.png)

SMOTE produced an accuracy score of 66%. 

3. Undersampling: 

![Undersampling_Classification Report](https://user-images.githubusercontent.com/113721712/230810050-6f1872df-23f7-4c63-b375-118501d2c6f4.png)

Undersampling produced an accuracy score of 52%. 

4. SMOTEEN

![SMOTEEN_Classification Report](https://user-images.githubusercontent.com/113721712/230810106-0452529d-33f4-4c09-bebc-a350e51cafe9.png)

SMOTEEN produced an accuracy score of 64%. 

5. Balanced Random Forest Classifier: 

![BRF_Classification Report](https://user-images.githubusercontent.com/113721712/230810178-068414ae-fb80-4470-8eb1-1fdf0a8fa8a3.png)

BRF produced an accuracy score of 78%. 

6. Easy Ensemble AdaBoost Classifier: 

![EEC_Classification Report](https://user-images.githubusercontent.com/113721712/230810244-f3ef064c-2c56-4d1a-ae93-4789ec6e73bd.png)

EEC produced an accuracy score of 93%. 

## Summary: 
It seems that none of the algorithms were able to efficiently predict credit card risk. While EEC produced a balanced accuracy score of 93%, and has high sensitivity (91%), its precision of high_risk predictions is 8%, meaning there were a lot of false positives. This means that a lot of people who are low_risk for a credit card would be misclassified as high_risk. Additionally, the f1 score for high_credit risk is 0.15 (the closer to 1, the better). This further demonstrates that there is a huge imbalance between precision and sensitivity. 


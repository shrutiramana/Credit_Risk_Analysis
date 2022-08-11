# Credit_Risk_Analysis

## Analysis Overview

The purpose of the project is to apply machine learning to solve a real-world challenge: credit card risk.Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we need to employ different techniques to train and evaluate models with unbalanced classes.We are required to - 
    1. Use Resampling Models to Predict Credit Risk
    2. Use the SMOTEENN Algorithm to Predict Credit Risk
    3. Use Ensemble Classifiers to Predict Credit Risk.
    
## Resources 

Data Source: LoanStats_2019Q1.csv
Software: Python, Anaconda Navigator,Conda, Jupyter Notebook

## Results 
### Naive Random Oversampling
![image](https://user-images.githubusercontent.com/98556229/184052529-48d8a4b7-09a8-4953-bf11-ee9892203152.png)

![image](https://user-images.githubusercontent.com/98556229/184052557-c1dc7e26-8025-46fc-a142-e1b994d73154.png)

The balanced accuracy score is 61%.
The high_risk precision is about 1% only with 62% sensitivity which makes a F1 of 1% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 61%.

    
### SMOTE Oversampling

![image](https://user-images.githubusercontent.com/98556229/184052719-8d50c9ff-c527-46c6-a49a-04019a8f7cad.png)

![image](https://user-images.githubusercontent.com/98556229/184052753-587f87b9-643d-48ac-a75c-debcc5ee01b3.png)

The balanced accuracy score is 62.25%.
The high_risk precision is about 1% only with 59% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 66%.



### Undersampling - CluseterCentroid.

![image](https://user-images.githubusercontent.com/98556229/184052889-c002c243-2cda-4ce8-a502-bb12e57cffa7.png)

![image](https://user-images.githubusercontent.com/98556229/184052911-ab9cce8f-8a21-40cb-9ea2-4b770dd2be32.png)

The balanced accuracy score is 52.4%.
The high_risk precision is about 0% only with 63% sensitivity which makes a F1 of 1% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 42%.


### SMOTEENN - Combination (Over and Under) Sampling

![image](https://user-images.githubusercontent.com/98556229/184053066-9347e6b0-8b4f-4866-a556-c38d3e4a1fa2.png)

![image](https://user-images.githubusercontent.com/98556229/184053082-f30c1cab-2f6b-4c97-9745-509ca57863d3.png)

The balanced accuracy score is 52.4%.
The high_risk precision is about 0% only with 63% sensitivity which makes a F1 of 1% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 42%.


### Balanced Random Forest Classifier

![image](https://user-images.githubusercontent.com/98556229/184054074-3f7c926b-a9ad-4433-9e66-7415fe270159.png)

![image](https://user-images.githubusercontent.com/98556229/184054089-1da6da2f-2eb2-46c9-86d6-c769ef649bf1.png)


The balanced accuracy score is 82.6%.
The high_risk precision is about 3% only with 77% sensitivity which makes a F1 of 6% .
Due to the high number of the low_risk population, its precision is almost 99% with a sensitivity of 88%.


### Easy Ensemble AdaBoost Classifier

![image](https://user-images.githubusercontent.com/98556229/184054214-2b7149e5-2929-4b0a-b1aa-48faf8aa4f73.png)

![image](https://user-images.githubusercontent.com/98556229/184054229-d23cb123-87c4-4e56-9729-7e2ca6b768e4.png)


## Summary
Six models Oversampling, Undersampling a, oversampled and combination of both , Balanced Random Forest Classifier and Easy Ensemble AdaBoost Classifier  to determine which is the best to predict the credit risk. For the first four models the accuracy score was not very high and also the high risk precision was also very low , indicating that they show that credit risk is high. The Ensemble models showed a lot of improvement in the accuracy to 92% and also it has low_risk precision to be 100% with recall of 95% and F1 is also 97%. Typically there should be a good balance of recall and precision.Easy Ensemble had the best balance of all. 














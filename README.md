# Credit_Risk_Analysis

## Purpose
The purpose of this challenge was to perform an analysis on credit card risk for applicants using data form LendingClub, a peer-to-peer lending service, using Machine Learning techniques in Python. Created models by using oversampling, undersampling, combination techniques with imbalanced-learn and scikit-learns libraries. 

## Results
### Resampling Results

* Oversampling: 
    
    - Random Oversampling
        - Classified 51,366 records each as High Risk and Low Risk. 
        ![image](https://user-images.githubusercontent.com/111200771/216797423-bce8d684-1021-4916-930c-3d77919e7c28.png)

 
    * Balanced Accuracy score = 66.5%
    * "High Risk" had a precision rate of 1%, recall of 72% and a model F1 score of 2%
    * "Low Risk" had a precision rate of 100%, recall of 61%.
    ![image](https://user-images.githubusercontent.com/111200771/216797434-42377385-11e5-4101-a9ee-1203da32d2fe.png)

![image](https://user-images.githubusercontent.com/111200771/216797450-3d3a37ac-c27a-44ca-aedb-30c7fa2401cd.png)


    - SMOTE Oversampling
        - Classified 51,366 records each as High Risk and Low Risk. 
    * Balanced Accuracy score = 65.3%
    * "High Risk" had a precision rate of 1%, recall of 63% and a model F1 score of 2%
    * "Low Risk" had a precision rate of 100%, recall of 68%.

* Undersampling

    - ClusterCentroids Resampling Module 
        - Classified 51,366 records each as High Risk and Low Risk. 

    * Balanced Accuracy score = 54.4%
    * "High Risk" had a precision rate of 1%, recall of 69% and a model F1 score of 1%
    * "Low Risk" had a precision rate of 100%, recall of 40%.

* Combination Sampling
    - SMOTEENN
        - Classified 68460 records as High Risk and 62011 as Low Risk. 

    * Balanced Accuracy score = 64.5%
    * "High Risk" had a precision rate of 1%, recall of 72% and a model F1 score of 2%
    * "Low Risk" had a precision rate of 100%, recall of 57%.


* Ensemble Learners
    - Classified 51366 records as Low Risk and 246 records as High Risk. 

    - Balanced Random Forest Classifier

    * Balanced Accuracy score = 79.3%
    * "High Risk" had a precision rate of 3%, recall of 70% and a model F1 score of 7%
    * "Low Risk" had a precision rate of 100%, recall of 88%.

    - Easy Ensemble Classifier

    * Balanced Accuracy score = 93.3%
    * "High Risk" had a precision rate of 9%, recall of 92% and a model F1 score of 16%
    * "Low Risk" had a precision rate of 100%, recall of 94%.

## Summary
After reviewing the results of the six different models, the EasyEnsembleClassifier model yeilded the best results with a precision rate of 9% and an accuracy score of 93.3% when predicting "High Risk" candidates. This model also yeild the best result for predicting "Low Risk" candidates with a sensitivity of 94% and an F1 score of 97%. The recommendation on which model to use when predicting the risk of loan candidates is to use the EasyEnsembleClassifier model. 

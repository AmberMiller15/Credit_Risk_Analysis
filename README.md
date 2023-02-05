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
        
    ![image](https://user-images.githubusercontent.com/111200771/216797509-7a837e54-8b28-4cad-9367-d6c55793a9a9.png)

   * Balanced Accuracy score = 65.3%
   * "High Risk" had a precision rate of 1%, recall of 63% and a model F1 score of 2%
   * "Low Risk" had a precision rate of 100%, recall of 68%.
   
    ![image](https://user-images.githubusercontent.com/111200771/216797538-8550ae48-5e92-4cc4-b735-7b4177d3243e.png)

    ![image](https://user-images.githubusercontent.com/111200771/216797545-582bfe4f-fb22-40a3-bced-fab694dcf731.png)

* Undersampling

    - ClusterCentroids Resampling Module 
        - Classified 246 records each as High Risk and Low Risk. 
        
    ![image](https://user-images.githubusercontent.com/111200771/216797553-1ba60058-7e10-4a87-9b2d-8a553ed7d95d.png)

    * Balanced Accuracy score = 54.4%
    * "High Risk" had a precision rate of 1%, recall of 69% and a model F1 score of 1%
    * "Low Risk" had a precision rate of 100%, recall of 40%.
 
    ![image](https://user-images.githubusercontent.com/111200771/216797578-8cec5047-1e98-469a-a34f-229771dec6d6.png)

    ![image](https://user-images.githubusercontent.com/111200771/216797587-0a1e0c31-649b-4a0a-8eb8-bdd1b6840f63.png)

* Combination Sampling
    - SMOTEENN
        - Classified 68460 records as High Risk and 62011 as Low Risk. 
        
    ![image](https://user-images.githubusercontent.com/111200771/216797594-10381f6f-3f43-4d07-b4a9-6f192ba25e2c.png)

    * Balanced Accuracy score = 64.5%
    * "High Risk" had a precision rate of 1%, recall of 72% and a model F1 score of 2%
    * "Low Risk" had a precision rate of 100%, recall of 57%.
    
    ![image](https://user-images.githubusercontent.com/111200771/216797606-53efab80-438c-41bc-8fd3-d478ede9f1c9.png)

    ![image](https://user-images.githubusercontent.com/111200771/216797609-20208064-4262-4629-be56-17d32942e87c.png)

* Ensemble Learners
    - Classified 51366 records as Low Risk and 246 records as High Risk. 
    
    ![image](https://user-images.githubusercontent.com/111200771/216797659-821d688c-dd7a-4347-9235-ec31a11e5006.png)
    
    - Balanced Random Forest Classifier

    * Balanced Accuracy score = 79.3%
    * "High Risk" had a precision rate of 3%, recall of 70% and a model F1 score of 7%
    * "Low Risk" had a precision rate of 100%, recall of 88%.
    
    ![image](https://user-images.githubusercontent.com/111200771/216797678-08a19824-cbb7-4fad-a620-78cd20e614bb.png)
    
    ![image](https://user-images.githubusercontent.com/111200771/216797683-dab2e6ef-8296-46dc-8bf9-cccdb7f0d798.png)

    - Easy Ensemble Classifier

    * Balanced Accuracy score = 93.3%
    * "High Risk" had a precision rate of 9%, recall of 92% and a model F1 score of 16%
    * "Low Risk" had a precision rate of 100%, recall of 94%.
    
    ![image](https://user-images.githubusercontent.com/111200771/216797700-0d350dc5-df6e-4c7b-baca-0a5d36f3ed9c.png)
    
    ![image](https://user-images.githubusercontent.com/111200771/216797724-cb569a69-2b41-4bb0-8aa6-3dc082feb1ba.png)

## Summary
After reviewing the results of the six different models, the EasyEnsembleClassifier model yeilded the best results with a precision rate of 9% and an accuracy score of 93.3% when predicting "High Risk" candidates. This model also yeild the best result for predicting "Low Risk" candidates with a sensitivity of 94% and an F1 score of 97%. The recommendation on which model to use when predicting the risk of loan candidates is to use the EasyEnsembleClassifier model. 

# **Task 10 – Analysis:**



## **1. Which model performed best?**

###### The best-performing model was the one with the highest cross-validation accuracy.

###### In most cases for this dataset, the tuned KNN model (with optimal k) or Logistic Regression performs best.

###### Based on results, the model with the highest mean CV score is selected as the best.

##### 

## **2. Did tuning improve performance?**

###### Yes, hyperparameter tuning improved performance.

###### When we tested different values of k in KNN, accuracy changed, and selecting the best k value gave better results than using a default value.

###### GridSearchCV further optimized the model and usually produced a higher or more stable accuracy.

###### 

## **3. Was cross-validation more reliable than a single split?**

###### Yes, cross-validation was more reliable.

###### A single train-test split depends on one random division of data, which can give biased results.

###### Cross-validation uses multiple splits (5-fold), so it provides a more consistent and accurate estimate of model performance.


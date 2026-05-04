# **Lab 09: Model Tuning \& Cross Validation**



### **Overview:**

This project applies multiple machine learning techniques on the Wine dataset from scikit-learn. The objective is to build, evaluate, and compare different models, apply hyperparameter tuning, and select the best-performing model.



### **Hyperparameter Tuning Process:**

Hyperparameter tuning was performed on the K-Nearest Neighbors (KNN) model to improve performance.



### **Manual Tuning:**

Different values of k (number of neighbors) were tested: 3, 5, 7, 9.

Each model was trained on the training data and evaluated on the test data.

Accuracy was recorded for each value, and the best k was selected based on highest accuracy.



### **GridSearchCV:**

GridSearchCV was used to automate the tuning process.

Parameter grid used: n\_neighbors = \[3, 5, 7, 9, 11]

5-fold cross-validation was applied to evaluate each parameter combination.

The best parameter and best cross validation score were selected.

This process helped in optimizing the model rather than relying on default parameters.



### **Model Comparison:**

Three models were compared using 5-fold cross-validation:

###### **Logistic Regression:** used as a baseline model

###### **KNN (tuned):** optimized using best k value

###### **Decision Tree:** a tree based classification model



### **Evaluation Method:**

Cross validation was used instead of a single train-test split to ensure reliable results.

Mean accuracy of each model was calculated.

### 

### **Observations:**

* Logistic Regression showed stable performance.
* Tuned KNN improved after selecting the optimal k value.
* Decision Tree performed adequately but was less consistent.
* ### 

### **Final Model Selection:**

The final model was selected based on the highest cross-validation accuracy.



### **Reasoning:**

Cross validation provides a more reliable performance estimate than a single split.

The model with the highest average accuracy across folds was chosen.

Hyperparameter tuning was considered to ensure fair comparison.



### **Conclusion:**

* Hyperparameter tuning improved model performance.
* Cross-validation provided more reliable evaluation.
* Comparing multiple models helped identify the best approach.
* The final model achieved the best balance of accuracy and consistency.




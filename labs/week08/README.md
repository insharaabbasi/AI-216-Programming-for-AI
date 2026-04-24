# Lab 08: Machine Learning Pipeline \& Model Evaluation



### Objective:

The objective of this lab is to build a complete machine learning workflow including:

\- Data loading and preprocessing  

\- Train-test splitting  

\- Training multiple machine learning models  

\- Evaluating model performance  

\- Comparing different models  

\- Understanding real-world ML pipeline structure  



### Dataset Description:

The Wine dataset is a built-in dataset from `scikit-learn`.



### Features:

\- Alcohol

\- Malic acid

\- Ash

\- Alcalinity of ash

\- Magnesium

\- Total phenols

\- Flavanoids

\- Nonflavanoid phenols

\- Proanthocyanins

\- Color intensity

\- Hue

\- OD280/OD315 of diluted wines

\- Proline



### Machine Learning Workflow:

#### 1.Data Loading:

\- Loaded Wine dataset using `sklearn.datasets.load\_wine`

\- Converted dataset into a Pandas DataFrame



#### 2.Data Preparation:

\- Separated features (X) and target (y)

\- Checked dataset shape and class distribution

#### 

#### 3.Train-Test Split:

\- Split dataset using 70% training and 30% testing

\- Used `random\_state=42` for reproducibility



### Models Implemented:

#### 1.Logistic Regression:

\- Linear classification model

\- Used for multi-class classification



#### 2.K-Nearest Neighbors (KNN):

\- Distance-based classification model

\- Used k = 5



#### 3.Decision Tree (Bonus Model):

\- Tree-based model

\- Handles non-linear relationships



### Model Evaluation Metrics:

The following evaluation metrics were used:

\- Accuracy Score  

\- Confusion Matrix  

\- Classification Report (Precision, Recall, F1-score)



### Key Observations:

\- Logistic Regression performs well when data is linearly separable  

\- KNN performance depends on distance and chosen k-value  

\- Decision Tree can capture complex patterns but may overfit  

\- Using more features improves accuracy compared to using a single feature  

\- Changing train-test ratio affects model generalization performance  



### Experiments Conducted:

#### 1.Feature Impact:

&#x20;   Model trained using:

&#x20; - Single feature (low accuracy)

&#x20; - All features (higher accuracy)



#### 2.Train-Test Ratio Impact:

\- 70/30 split vs 50/50 split

\- More test data reduced training performance slightly



### Conclusion:

This lab demonstrates a complete machine learning pipeline:

\- Data preprocessing  

\- Model training  

\- Model comparison  

\- Performance evaluation  



It highlights that different models behave differently depending on data structure, and proper evaluation is necessary before selecting a final model.






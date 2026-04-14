## AI-216 Week 7 Lab – Data Preprocessing Pipeline



In this lab, I worked on preparing a raw hiring dataset for machine learning. The dataset contained missing values, inconsistent categorical entries, and non-numeric features. The main goal was to clean, transform, and normalize the data so it could be used for a predictive model.

I built a complete preprocessing pipeline that handles missing values, standardizes categorical data, engineers new features, and normalizes numeric columns in a reusable function.



#### Tasks Summary:

##### 

##### Task 1 – Load and Inspect Data:

Loaded CSV and JSON files into Pandas DataFrames and performed initial inspection using .head(), .dtypes, .shape, and .isnull().sum() to understand data quality issues.



#### Task 2 – Merge Datasets:

Merged both datasets using id as the key to combine applicant details with their skills and education information.



#### Task 3 – Handle Missing Values:

* Filled missing age values using median
* Replaced missing experience with 0
* Converted "?" in expected\_salary to NaN and filled with median
* Filled missing education with "Unknown"
* Handled missing name by keeping it as "Unknown" since it is not useful for model training



#### Task 4 – Clean Inconsistent Data:

Standardized the city column by:

* Replacing "isl" with "Islamabad"
* Converting all city names to lowercase for consistency



#### Task 5 – Feature Engineering:

Created a new column experience\_level using:

* 0–1 years → junior
* 2–5 years → mid
* 6+ years → senior



#### Task 6 – Normalize Numeric Features:

Applied Min-Max normalization to:

* age
* experience
* expected\_salary

All values were scaled between 0 and 1.



#### Task 7 – Preprocessing Function:

Created a reusable function preprocess\_applicants(df) that:

* Handles missing values
* Cleans categorical data
* Creates experience\_level
* Normalizes numeric columns
* Returns a fully cleaned dataset



### Key Decisions \& Reasoning:



#### 1\. Using Median Instead of Mean:

I used the median for filling missing values in age and expected\_salary because median is more robust to outliers. In real-world salary data, extreme values can heavily skew the mean, making median a safer choice.



#### 2\. Filling Missing Experience with 0:

I assumed missing experience means the applicant likely has no recorded professional experience. While this may not always be perfectly accurate, it provides a reasonable baseline for modeling.



#### Surprise / Challenge:

One challenge was dealing with inconsistent categorical data in the city column. Values like "isl", "Islamabad", and different casing required careful standardization. I initially missed case inconsistencies, which showed that Pandas does not automatically normalize text data.



#### Q:If 100 new applicants are submitted, I would need to ensure?

* The same preprocessing function is applied consistently
* The median values used for missing data should ideally be stored from the training dataset instead of recalculating every time
* The encoding rules (city standardization, experience levels) remain fixed and do not change with new data
* The pipeline should be deployed as a reusable function or part of an ML pipeline (e.g., scikit-learn Pipeline)



This lab helped me understand that preprocessing is not just cleaning data, it is about making consistent, logical decisions that directly affect model performance.


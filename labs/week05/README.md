# **AI-216 – Programming for Artificial Intelligence**  

# **Lab 5**



**Objective:**

Learn to use NumPy and Pandas to process and analyze data efficiently.



#### **Difference Between NumPy \& Pandas**

\- **NumPy:** Works with arrays and matrices, great for fast numeric calculations and vectorized operations.  

\- **Pandas:** Works with tables (DataFrames), ideal for data cleaning, filtering, grouping, and CSV handling.  



#### **Why Vectorization is Preferred**

\- Vectorized operations handle entire arrays or columns at once.  

\- Avoids slow loops and makes code faster and simpler.  



#### **How Missing Data Was Handled**

\- Checked for missing values using isnull()

\- Replaced missing Amount values with the median using fillna() 

\- Ensured data type consistency by converting Amount to integer  



#### **Part A: NumPy**

* We used NumPy to work with numbers in arrays and matrices.
* We had a sensor data matrix for machines over time.
* We found average readings for each machine and maximum readings for each time.
* We normalized the numbers by dividing each value by the column maximum.
* We used boolean indexing to find machines with high average readings.
* We reshaped the matrix into a new shape.
* We also created random matrices, did matrix multiplication, element-wise multiplication, filtered numbers, and stacked matrices together.



#### **Part B: Pandas**

* We used Pandas to work with tables of data (DataFrames).
* We loaded an e-commerce dataset.
* We checked for missing values and filled missing amounts with the median.
* We converted Amount to integers.
* We added a HighValue column for orders greater than 10000.
* We filtered orders by city and category, and sorted by Amount.
* We found the top customers by total spending.
* We did grouping and aggregation to find total revenue, average order, and unique customers.
* We created a pivot table for City vs Category.
* Advanced: we added TaxedAmount, made city names lowercase, removed duplicate customers keeping the highest purchase, and created a summary dictionary.
* Finally, we exported the cleaned data to a CSV file.

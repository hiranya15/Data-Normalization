# STUDY OF DATA NORMALIZATION AND CATEGORICAL ENCODING USING PYTHON
 
Name – Hiranya

Branch – ENTC A3

PRN – 25070123054

# ▲ Aim

To study and implement data normalization techniques and encoding of categorical variables using Python.

# ▲ Introduction

In data analysis and machine learning, datasets often contain numerical values with varying scales along with categorical variables. These differences can negatively impact the performance of analytical models.

Data normalization is used to bring numerical values to a common scale, while categorical encoding converts non-numeric data into numerical form so that it can be processed by machine learning algorithms.

Python libraries such as Pandas, NumPy, and Scikit-learn provide efficient and reliable methods to perform these preprocessing operations.

# ▲ Theory
Data Normalization

Data normalization is the process of scaling numerical values to a standard range so that no single feature dominates others. It improves model performance and ensures balanced comparison between variables.

The commonly used normalization techniques are:

Min-Max Normalization
This technique scales values between 0 and 1 using the formula:
(x - min) / (max - min)
It is suitable when the dataset does not contain extreme outliers.
Z-Score Normalization
This method standardizes data using mean and standard deviation:
(x - mean) / std
It is effective when the dataset contains outliers.
Decimal Scaling
This method scales values by dividing them by powers of 10, reducing them to a smaller range.

Normalization can also be applied to multiple columns simultaneously using vectorized operations in Pandas.

Categorical Encoding

Categorical variables cannot be directly used in numerical analysis. Therefore, they must be converted into numerical form using encoding techniques.

Label Encoding
Assigns a unique integer to each category.
Example: Male = 1, Female = 0
One-Hot Encoding
Creates separate binary columns for each category using pd.get_dummies().
Dummy Encoding
Similar to one-hot encoding but removes one column to avoid redundancy and multicollinearity.

These techniques allow categorical data to be used effectively in machine learning models.

# ▲ Procedure
Import required libraries such as Pandas, NumPy, and Scikit-learn.
Create a dataset containing numerical and categorical features.
Apply Min-Max normalization to numerical columns.
Apply Z-score normalization using mean and standard deviation.
Perform decimal scaling on numerical data.
Normalize multiple columns simultaneously.
Create a dataset containing categorical variables.
Apply Label Encoding using LabelEncoder.
Apply One-Hot Encoding using pd.get_dummies().
Apply Dummy Encoding by dropping one column.
Load a larger dataset (Amazon dataset).
Apply normalization techniques on price and rating columns.
Analyze and verify the transformed dataset.
# ▲ Observations / Result
Price values were successfully scaled between 0 and 1 using Min-Max normalization.
Units sold were standardized using Z-score normalization.
Decimal scaling reduced large numerical values to smaller ranges.
Multiple columns were normalized simultaneously.

For categorical data:

Gender was encoded using Label Encoding (Male = 1, Female = 0).
Payment method was converted into binary columns using One-Hot Encoding.
Dummy encoding reduced redundancy by removing one column.

For the larger dataset:

Price and rating values were effectively normalized.
The final dataset became consistent, scaled, and suitable for machine learning applications.
# ▲ Tools / Libraries Used
Python
Google Colab / Jupyter Notebook
Pandas
NumPy
Scikit-learn
# ▲ Applications
Data preprocessing in machine learning
Improving model performance through scaling
Converting categorical data into usable numerical form
Data analytics and business intelligence
Customer and sales data analysis
# ▲ Advantages
Improves accuracy of machine learning models
Ensures all features are on a uniform scale
Reduces bias caused by large numerical values
Converts categorical data into numerical format
Enhances data consistency and usability
# ▲ Conclusion

Data normalization and categorical encoding are essential preprocessing techniques in data analysis and machine learning. Normalization ensures that numerical data is scaled appropriately, while encoding transforms categorical variables into numerical form. Using Python libraries such as Pandas and Scikit-learn, these operations can be performed efficiently, making the dataset suitable for further analysis and model building.

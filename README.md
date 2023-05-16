# Ex03-Univariate-Analysis
# Aim
To read the given data and perform the univariate analysis with different types of plots
# Explanation
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.
# Algorithm
# Step1
Read the given data.
# Step2
Get the information about the data.
# Step3
Remove the null values from the data.
# Step4
Mention the datatypes from the data.
# Step5
Count the values from the data.
# Step6
Do plots like boxplots,countplot,distribution plot,histogram plot.
# Program
```
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv('superstore.csv')
df
df.head()
df.info()
df.describe()
df.isnull().sum()
df.dtypes
df['Postal Code'].value_counts()
sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
sns.histplot(x='Postal Code',data=df)
```
# OUTPUT
# DATA
![image](https://github.com/Sahithya7/Ex03-Univariate-Analysis/assets/133002193/061bfe3d-5f0a-4f4f-ad26-d8a9f39595a6)
# DATA HEAD
![image](https://github.com/Sahithya7/Ex03-Univariate-Analysis/assets/133002193/cc67cb16-3098-4789-8580-e884124704be)
# DATA INFORMATION
![image](https://github.com/Sahithya7/Ex03-Univariate-Analysis/assets/133002193/a91037a6-2105-4a22-8859-4b0138c9ef3a)
# DATA DESCRIBE
![image](https://github.com/Sahithya7/Ex03-Univariate-Analysis/assets/133002193/894ffd14-aada-450e-877b-7e2c470fa13b)
# DATA NULL VALUES
# DATA'S DATATYPES
# DATA'S VALUECOUNT
![image](https://github.com/Sahithya7/Ex03-Univariate-Analysis/assets/133002193/4c1c85cf-7bb8-4b30-8e55-16387f2657df)
# BOXPLOT
# COUNTPLOT
# DISTRIBUTION PLOT
# HISTOGRAM PLOT
# Result
Thus we have read the given data and performed the univariate analysis with different types of plots.

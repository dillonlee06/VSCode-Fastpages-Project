---
toc: true
layout: post
categories: [AP Notes, CSP Assignments]
title: Data Analysis Hacks
---
> Questions (0.9)
- What are the two primary data structures in pandas and how do they differ?
- Series and DataFrame are the two main types of data structures in pandas. While DataFrame is a two-dimensional labeled data structure with columns of potentially different data types, similar to a spreadsheet or SQL table, Series is a one-dimensional labeled array that can hold any data type.
- How do you read a CSV file into a pandas DataFrame?
- Use the read_csv() function offered by pandas to read a CSV file into a pandas DataFrame. The data from the CSV file is returned in a DataFrame object by this function, which accepts the file path of the CSV file as input.
- How do you select a single column from a pandas DataFrame?
- You can use bracket notation and provide the name of the column you wish to pick as a string to select a single column from a pandas DataFrame. You can use the syntax df["column_name"] to choose the column in a DataFrame with the name "column_name," for instance.
- How do you filter rows in a pandas DataFrame based on a condition?
- Boolean indexing can be used to filter rows in a pandas DataFrame according to a criterion. To pick the rows that meet the condition, you can apply a conditional statement to one or more columns in the DataFrame to build a boolean mask. This boolean mask is then passed to the DataFrame's indexing operator ([]). For instance, the expression df[df['column_name'] > 10] will produce a new DataFrame that only contains the rows where the value of "column_name" exceeds 10.
- How do you group rows in a pandas DataFrame by a particular column?
- By passing the column name as an argument to the groupby() method of the DataFrame object, you can group the rows in a pandas DataFrame by a certain column. By doing this, a new DataFrameGroupBy object will be created, which you can then modify to aggregate or summarize the data for each group. For instance, df.groupby('column_name') groups the rows of the DataFrame df according to the distinct values in the 'column_name' column.
- How do you aggregate data in a pandas DataFrame using functions like sum and mean?
- To aggregate data in a pandas DataFrame using functions like sum and mean, you can use the agg() method of the DataFrameGroupBy object returned by groupby().
- How do you handle missing values in a pandas DataFrame
You can use functions like isna() or isnull() to find missing values in a pandas DataFrame, and then you can use functions like dropna() or fillna() to either remove the rows or fill in the missing values with a specified value or method.
- How do you merge two pandas DataFrames together?
- You can use the merge() function supplied by pandas to combine two pandas DataFrames by specifying the columns or indices to merge on, the kind of join to employ, and any extra merge settings. For instance, pd.merge(df1, df2, on='column_name', how='inner') will use an inner join to combine two DataFrames df1 and df2 on the shared column 'column_name'.
- How do you export a pandas DataFrame to a CSV file?
- To export a pandas DataFrame to a CSV file, you can use the to_csv() method of the DataFrame object and specify the file path and name for the CSV file.
- What is the difference between a Series and a DataFrame in Pandas?
- The main difference between a Series and a DataFrame in Pandas is that a Series is a one-dimensional labeled array that can hold any data type, while a DataFrame is a two-dimensional labeled data structure with columns of potentially different data types, similar to a spreadsheet or SQL table.

> Data Analysis / Predictive Analysis (0.9)
- How can Numpy and Pandas be used to preprocess data for predictive analysis?
- By offering strong capabilities for data manipulation and transformation, including as cleaning and normalization, missing value management, feature engineering, and more, Numpy and Pandas can be used to preprocess data for predictive analysis. In order to prepare data in a format that machine learning algorithms can use, these libraries can be used.
- What machine learning algorithms canThere are several machine learning techniques that can be used for predictive analysis, each with specific strengths and shortcomings, such as linear regression, decision trees, random forests, support vector machines, and neural networks. be used for predictive analysis, and how do they differ?\
- There are several machine learning techniques that can be used for predictive analysis, each with specific strengths and shortcomings, such as linear regression, decision trees, random forests, support vector machines, and neural networks.
- Can you discuss some real-world applications of predictive analysis in different industries?
- Numerous real-world applications of predictive analysis can be found in a variety of industries, including predicting equipment failures in manufacturing and healthcare, customer churn in telecommunications and finance, retail and e-commerce demand, energy usage and price forecasting in utilities, and credit risk forecasting in banking and finance.
- Can you explain the role of feature engineering in predictive analysis, and how it can improve model accuracy?
- The predictive model's dependability and accuracy will increase thanks to feature engineering. Feature selection is one method that feature engineering is put into practice so that you only receive the most crucial data.
- How can machine learning models be deployed in real-time applications for predictive analysis?
- By developing an API that receives input data, applies the model to make predictions, and returns the results to the application in real-time, machine learning models can be implemented in real-time applications for predictive analysis.
- Can you discuss some limitations of Numpy and Pandas, and when it might be necessary to use other data analysis tools?
- When working with complex data structures, Numpy and Pandas' memory requirements, as well as their relatively slow performance, are some of their drawbacks. They also offer limited support for some advanced analytical techniques, such as deep learning, which may call for specialized software and frameworks.
- How can predictive analysis be used to improve decision-making and optimize business processes?
- Predictive analysis can be used to improve decision-making and optimize business processes by providing insights and recommendations based on historical data, allowing organizations to make more informed and data-driven decisions.

# EDA_ON_DIWALI_SALES

Importing Libraries:
The code begins by importing the necessary Python libraries for data analysis and visualization. These libraries include:

numpy (as np) for numerical computing in Python.
pandas (as pd) for data manipulation and analysis using DataFrames.
matplotlib.pyplot (as plt) for visualizing data through various plots.
seaborn for creating more visually appealing and informative statistical graphics.

Loading the Data:
The code reads the Diwali sales data from the CSV file 'Diwali_Sales_Data.csv' into a Pandas DataFrame called df. It uses pd.read_csv() function to achieve this. Additionally, it uses the 'unicode_escape' encoding to handle any special characters present in the CSV file.

Data Exploration:
The code performs initial exploration of the data:
It displays the shape of the DataFrame using df.shape to show the number of rows and columns.
It shows the first few rows of the DataFrame using df.head() to get a glimpse of the data.
It prints the summary of the DataFrame using df.info() to get information about the data types and non-null values in each column.

Data Cleaning:
Drop Unrelated Columns:
The code drops two columns, 'Status' and 'unnamed1', from the DataFrame using df.drop(). These columns are considered unrelated to the analysis and are removed from the DataFrame to focus on relevant data.

Handling Null Values:
The code checks for null values in the DataFrame using pd.isnull(df).sum() to count the number of missing values in each column. It then drops rows containing null values using df.dropna().

Data Type Conversion:
The code converts the 'Amount' column to the integer data type using df['Amount'] = df['Amount'].astype('int'). This conversion is useful for performing numerical calculations and visualizations on the 'Amount' column.

Column Renaming (Not Applied):
The code renames the 'Marital_Status' column to 'Shaadi' using df.rename(columns={'Marital_Status':'Shaadi'}). However, this renaming is not applied to the DataFrame itself, so the column name remains unchanged.

Statistical Description:
The code uses df.describe() to generate a statistical summary of the data in the DataFrame. It provides statistical measures like count, mean, standard deviation, minimum, 25th percentile, median (50th percentile), 75th percentile, and maximum for all numeric columns in the DataFrame.

Specific Column Descriptions:
The code uses df[['Age', 'Orders', 'Amount']].describe() to generate a more focused statistical summary for specific columns: 'Age', 'Orders', and 'Amount'. This helps in understanding the distribution of these individual columns.
Data Visualization:
The code uses various Seaborn and Matplotlib functions to visualize the data and gain insights from it. It creates different types of bar charts, each with a specific focus:

Gender vs. Count: The code plots a countplot (bar chart) to visualize the distribution of genders and their counts in the dataset.

Gender vs. Total Amount: The code uses a barplot to compare the total amount of sales between different genders.

Gender vs. Count by Age Group: The code creates a grouped countplot to visualize the count of each gender within different age groups.

Age Group vs. Total Amount: The code uses a barplot to display the total amount of sales for each age group.

Top 10 States: The code calculates and plots the total number of orders and total amount of sales for the top 10 states with the highest values.

Marital Status: The code plots a countplot to show the count of individuals with different marital statuses.

Marital Status vs. Total Amount by Gender: The code creates a barplot to compare the total sales amount for each gender within different marital statuses.

Occupation: The code plots a countplot to visualize the count of individuals belonging to different occupations.

Occupation vs. Total Amount: The code uses a barplot to show the total amount of sales for each occupation.

Product Category: The code plots a countplot to visualize the count of sales for each product category.

Product Category vs. Total Amount: The code creates a barplot to display the total amount of sales for the top 10 product categories.

Top 10 Product IDs: The code calculates and plots the total number of orders for the top 10 product IDs.

Additional Visualization:
The code uses Matplotlib to create a bar chart to show the sum of orders for the top 10 product IDs in a single plot.

The code presents a comprehensive analysis of the Diwali sales data, exploring various aspects such as gender distribution, age groups, states with the highest sales, marital status, occupation, and top-selling product categories and products. These visualizations provide valuable insights into the dataset and help understand sales patterns and trends effectively.

# EDA_ON_DIWALI_SALES

This Python code utilizes various data manipulation and visualization techniques to analyze Diwali sales data from a CSV file ('Diwali_Sales_Data.csv'). The code performs the following steps:

Import necessary Python libraries, including NumPy, Pandas, Matplotlib, and Seaborn, for data analysis and visualization.

Read the CSV file into a Pandas DataFrame, examine its shape, and display the first few rows and info about the data.

Drop unrelated/blank columns ('Status' and 'unnamed1') from the DataFrame.

Check for and drop null values from the DataFrame.

Convert the 'Amount' column to an integer data type.

Rename the 'Marital_Status' column to 'Shaadi' (though the renaming is not applied to the DataFrame).

Perform statistical descriptions using the describe() method on the DataFrame and specific columns ('Age', 'Orders', and 'Amount').

Visualize the data using different types of plots, including bar charts, to gain insights into sales patterns:

a. Plot the count of each gender in the dataset.

b. Plot the total amount of sales for each gender.

c. Plot the count of each age group by gender.

d. Plot the total amount of sales for each age group.

e. Plot the total number of orders from the top 10 states.

f. Plot the total amount of sales from the top 10 states.

g. Plot the count of individuals with different marital statuses.

h. Plot the total amount of sales for each gender within different marital statuses.

i. Plot the count of individuals belonging to different occupations.

j. Plot the total amount of sales for each occupation.

k. Plot the count of sales for the top 10 product categories.

l. Plot the total amount of sales for the top 10 product categories.

m. Plot the total number of orders for the top 10 product IDs.

n. Plot the sum of orders for the top 10 product IDs in a bar chart.

The code creates multiple visualizations to help understand the distribution of sales data based on various attributes like gender, age group, state, marital status, occupation, product category, and product ID.

# Pandas_1
I've continued my Python/Pandas journey by learning data preparation and EDA. I've used titanic dataset and crosstab() function to cross-examination for any two columns. I've used groupby() and agg() function to group columns' values by aggregating based on another column just like Group By Key in SQL. If we use groupby() method, our index values turn into the values that specified in groupby(). We could avoid this situation by using .rest_index(). That way, we can turn our index values into integers again (starting by 0, of course) . We can use isnull() and sum() methods altogether to see whether any columns have null values. Also we can use count(), sum() etc for mathematical and statistical operations. 

A column may have different values. We might want to see how many values this column has. Especially for categorical columns. So, We can use value_counts() method to see or we can see value_counts() and .shape[0] altogether to see as percentage and I think we should separate numerical and categorical columns from each other that can be found altogether in df.columns to analyze our dataset better.

We can use .dtypes and info() to see dataset's columns' types and whether they have null values. We use .read_csv() method to get dataset from excel that has a .csv extension. We should use .copy() method for avoid changing main dataset. That way, we may use the copy of the main dataset.

Creating a new column in a dataset is easy. 
dataset["new_column_name"] = new_value format will be enough but all records will have the same value for that column. We can change this values by using loops, conditions etc

Another important keywords are .loc and .iloc. We can use these to get subdatasets from main dataset by using column name or index values to specify these columns and rows. We can use .loc to create a new column that has different values based on a condition too.

We use .fillna() method to change a column's null values with another values such as the values of this column's median(). We generally don't like null values, they might make our further analyses (especially in ML) difficult.

With .to_csv() method we can send our dataset from Jupyter/Python to Excel as a csv file. And also, we can use .sort_values() method to apply ascending/descending ordering on a dataset based on some columns' values.  


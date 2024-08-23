### Developed By: VINOD KUMAR S
### Register No: 212222240116
### Date:

# Ex.No: 01A PLOT A TIME SERIES DATA



# AIM:

To Develop a python program to Plot a time series data on Coffee Sales



# ALGORITHM:


 1.Import the necessary libraries: Import pandas, numpy, and matplotlib.pyplot.
 
 2.Load the CSV data: Use pandas.read_csv to load the first 50 rows of the data from index.csv into a DataFrame.
 
 3.Preview the data: Use DataFrame.head() to display the first 10 rows of the DataFrame.
 
 4.Group and count data: Group the data by date and coffee_name, then count the occurrences for each group.
 
 5.Create the plot: Use matplotlib to create a line plot that shows the count of each coffee_name by date.
 
 6.Customize the plot: Add a title, labels, and rotate the x-axis labels for better readability.
 
 7.Display the plot: Use plt.show() to display the final plot.
  <br />
   <br />


# PROGRAM:



```python

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
df=pd.read_csv("index.csv",nrows=50)
df.head(10)
plt.plot(df.date,df.coffee_name)
plt.title("classes by date")
plt.xlabel("date")
plt.xticks(rotation=45)
plt.ylabel("coffee name")

```
 <br />
 <br />
# OUTPUT:


![Screenshot 2024-08-16 093407](https://github.com/user-attachments/assets/f00d4b00-d8dc-434e-971b-3531dc889ebb)



# RESULT:
Thus we have created the python code for plotting the time series of given data.

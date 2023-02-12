# france-housing-salary

  # housing
 collection of information about various towns and cities in France, including the name of the town, its population, the number of sales, and the average price per square meter of housing. The data is read into a Pandas DataFrame and some basic statistical analysis is performed on the price column to describe the distribution. Boxplots are generated to visualize the distribution of prices across different regions of France, and the influence of the town's population on the housing prices is also explored.
 
 The given code is in Python and uses the pandas and seaborn libraries. The first step is to import the required libraries and read the data from a csv file using pd.read_csv and store it in a pandas dataframe T. The head() function is then used to display the first few rows of the data.

The data is then filtered to keep only the rows where the pop column is greater than 2000 and stored in a new dataframe S. The describe() function is then used to get the descriptive statistics of the prix column.

Two plots are then created using the seaborn library. The first plot is a simple box plot of the prix column, and the second plot is a box plot of prix against the reg column, with different regions separated by color. The whis parameter is set to [0,100] to remove outliers and the showmeans parameter is set to True to display the mean values.

A third plot is then created, which is similar to the second plot but with an additional hue based on the grande column, which indicates whether the population is greater than or equal to 2000. The code creates this column by using the apply function and a lambda function to create a new column based on the values in the pop column.

  # lorenz curv
  
The code above is analyzing income data for a specific department (77) in France. The data is loaded into a pandas dataframe using the read_csv function.

Next, the code creates cumulative sums of the number of households (Foyers) and the total income (Mas_rev) using the cumsum function. These cumulative sums are stored in the columns 'ECC_f' and 'ECC_r' respectively.

The code then calculates the average income per household using the division operator. The total number of households and total income are also computed and stored in the variables 'F' and 'R'.

Finally, the Lorenz curve is plotted using the plot function from the pylab library. The curve displays the cumulative frequency of households (FCC_f) on the x-axis and cumulative income (FCC_r) on the y-axis. The plot is customized with markers, labels, grid lines, and annotations for each data point. The plot style is set using the "bmh" style from the pylab library.

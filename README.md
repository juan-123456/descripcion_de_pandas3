# descripcion_de_pandas3

+ import pandas as pd: we import the necessary libraries.

+ drinks = pd.read_csv('https://raw.githubusercontent.com/justmarkham/DAT8/master/data/drinks.csv')
drinks.head(): let´s get the address where the database is a name and show the table.

+ drinks.groupby('country').beer_servings.mean(): what it does is search as a link, which shows country with beer_servings data.

+ drinks.groupby('continent').wine_servings.describe(): 
this function shows in addition to the average also shows part of the median along with its other filters such as those that are most requested, the total percentage, median percentage, etc. unlike the mean is that this shows everything in addition to the mean (mean) doing A link type between tables.

+ drinks.groupby('continent').mean(): print the average of what you select but for each column in general.

+ drinks.groupby('continent').median(): shows the median of the selected column.

+ drinks.groupby('continent').spirit_servings.agg(['mean', 'min', 'max']): it shows the average values, minimum and maximum values.

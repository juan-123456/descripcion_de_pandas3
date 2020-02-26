# descripcion_de_pandas3

+ import pandas as pd: importamos las librerias necesarias.

+ drinks = pd.read_csv('https://raw.githubusercontent.com/justmarkham/DAT8/master/data/drinks.csv')
drinks.head(): asiganmos la direccion donde esta la base de datos un nombre y mostramos la tabla.

+ drinks.groupby('country').beer_servings.mean(): lo que hace es buscar como un enlace, que muestre country con los datos de beer_servings.

+ drinks.groupby('continent').wine_servings.describe(): esta funcion muestra ademas de la media tambien muestra parte de la mediana junto con sus demas filtros como los que mas se piden, el porcentraje total, porcentaje mediana, etc a diferencia del mean es que este muestra todo ademas de la mean (media) haciendo un tipo enlace entre tablas.

+ drinks.groupby('continent').mean(): imprime la media de lo que selecciones pero de cada columna en general.

+ drinks.groupby('continent').median(): muestra la mediana de la columna seleccionada.

+ drinks.groupby('continent').spirit_servings.agg(['mean', 'min', 'max']): muestra los valores de media, valores minimos y maximos.

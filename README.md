# Predicting-House-Prices
Objective: To predict house prices based on area using linear regression model.

## Python Library:
Pandas, Numpy, Matplotlib, Sklearn

## Method: 
```sql
import pandas as pd
import numpy as np 
import matplotlib.pyplot as plt
from sklearn import linear_model
```

```sql
#removing any extra spaces from the column names
df= pd.read_excel('data.xlsx')
df.columns = df.columns.str.strip()
```

```sql
%matplotlib inline
plt.xlabel('Area(sqr ft)')
plt.ylabel('Prices(US$)')
plt.scatter(df.Area, df.Prices, color= 'red', marker= '+')
plt.show()
```

```sql
# Creating object for linear regression
reg = linear_model.LinearRegression()
reg.fit(df[['Area']], df.Prices)
```

```sql
reg.predict([[3300]])
```




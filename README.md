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

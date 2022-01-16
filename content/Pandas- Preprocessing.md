# Pandas: Preprocessing
```python
from sklearn.compose import ColumnTransformer
from sklearn.pipeline import Pipeline
from sklearn.impute import SimpleImputer
from sklearn.preprocessing import OneHotEncoder

# Preprocessing for numerical data
numerical_transformer = SimpleImputer(strategy='constant')

# Preprocessing for categorical data
categorical_transformer = Pipeline(steps=[
    ('imputer', SimpleImputer(strategy='most_frequent')),
    ('onehot', OneHotEncoder(handle_unknown='ignore'))
])

# Bundle preprocessing for numerical and categorical data
preprocessor = ColumnTransformer(
transformers=[
	('num', numerical_transformer, numerical_cols), 
	('cat', categorical_transformer, categorical_cols)
])

from sklearn.ensemble import RandomForestRegressor

model = RandomForestRegressor(n_estimators=100, random_state=0)

my_pipeline = Pipeline(steps=[('preprocessor', preprocessor), ('model', model)])
```



<!-- #anki/tag/Python #anki/deck/Programming -->

<!-- {BearID:FA018E26-72FF-4462-83F9-B60B2CA6DFDF-78674-00000426AAF14779} -->

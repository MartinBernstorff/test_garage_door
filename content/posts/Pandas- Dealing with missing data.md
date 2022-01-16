# Pandas: Dealing with missing data
See also [[Pandas: Preprocessing]]

Q. How might we generate a list of columns with missing values in pandas?
A. 
```
cols_with_missing = [col for col in X_train.columns
                     if X_train[col].isnull().any()]
```

Examine missing values by column:
```
missing_val_count_by_column = (X_train.isnull().sum())
```

To drop all columns with missing values:
```
cleaned_data = df.drop(cols=cols_with_missing)
```

# Continuous variables
To do simple median or mean imputation:
```
from sklearn.impute import SimpleImputer

imputer = SimpleImputer(strategy="mean")

imputed_X_train = pd.DataFrame(imputer.fit_transform(X_train), columns=X_train.columns)
imputed_X_valid = pd.DataFrame(imputer.fit(X_train).transform(X_valid), columns=X_valid.columns)

```
<!-- #anki/tag/Python #anki/deck/Programming -->

<!-- {BearID:0530554E-A8E1-4634-8ADD-53E32D249DFF-78674-0000040795169960} -->

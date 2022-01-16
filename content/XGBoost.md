# XGBoost
```
my_model = XGBRegressor(n_estimators=1000, 
	learning_rate=0.05, 
	n_jobs=4)

my_model.fit(X_train, y_train, 
             early_stopping_rounds=5, 
             eval_set=[(X_valid, y_valid)], 
             verbose=False)
```

Parameters to grid-search:
1. Learning_rate
2. n_estimators
3. early_stopping_rounds

## Backlinks
* [[Gradient boosting]]
	* One example of this is [[XGBoost]].

<!-- {BearID:402A50A7-91F2-4AA3-BC1F-D344BF83812E-42740-00000296A0DE5AA9} -->

# ML: Define a random forest
```
from sklearn.ensemble import RandomForestRegressor
from sklearn.metrics import mean_absolute_error

model = RandomForestRegressor(random_state=1)

model.fit(train_X, train_y)

melb_preds = model.predict(val_X)

print(mean_absolute_error(val_y, melb_preds))
```

<!-- {BearID:C60AE24E-96B0-493D-94F8-2C11EE407F80-60700-00000365C2AEB02E} -->

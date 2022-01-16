# Sklearn: Cross-validation (grid search)
```
from sklearn.model_selection import cross_val_score

# Multiply by -1 since sklearn calculates *negative* MAE
scores = -1 * cross_val_score(my_pipeline, X, y, cv=5, scoring='neg_mean_absolute_error')

print("MAE scores:\n", scores)

print("Average MAE score (across experiments):")
print(scores.mean())
```

<!-- #anki/tag/Python #anki/deck/Programming -->

<!-- {BearID:76B6178A-5DA7-4398-A71B-3CC3DE69E671-78674-0000042FBE308E02} -->

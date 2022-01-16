# Algorithm selection and design for ML
## Shortlist Promising Models
Notes:
* If the data is huge, you may want to sample smaller training sets so you can train many different models in a reasonable time (be aware that this penalizes complex models such as large neural nets or Random Forests).

```
y = df.Column # Select prediction target

features = ["col 1", "col 2"]
X = df[features] # Select features
```

# Define
[[ML: Defining a decision tree]]
[[ML: Define a random forest]]

# Fit and predict
`model.fit(X, y)`
`predictions = model.predict(X)`

# Evaluate
Remember to use your validation set from [[Collect data for ML]].

```
val_predictions = model.predict(val_X)
```


### Mean absolute error
```
from sklearn.metrics import mean_absolute_error

mean_absolute_error(y, val_predictions)
```

[[Sklearn: Cross-validation (grid search)]]

1. Train many quick-and-dirty models from different categories (e.g., linear, naive Bayes, SVM, Random Forest, neural net, etc.) using standard parameters.



3. Measure and compare their performance.
	* For each model, use N-fold cross-validation and compute the mean and standard deviation of the performance measure on the N folds.
3. Analyze the most significant variables for each algorithm.
4. Analyze the types of errors the models make.
	* What data would a human have used to avoid these errors?
5. Perform a quick round of feature selection and engineering.
6. Perform one or two more quick iterations of the five previous steps.
7. Shortlist the top three to five most promising models, preferring models that make different types of errors.

## Fine-tune the system
* You will want to use as much data as possible for this step, especially as you move toward the end of fine-tuning.

* As always, automate what you can.

1. Fine-tune the hyperparameters using cross-validation:
	* Treat your data transformation choices as hyperparameters, especially when you are not sure about them (e.g., if you’re not sure whether to replace missing values with zeros or with the median value, or to just drop the rows).
	* Unless there are very few hyperparameter values to explore, prefer random search over [[Sklearn: Grid search]]. 
		* If training is very long, you may prefer a Bayesian optimization approach (e.g., using Gaussian process priors, as described by Jasper Snoek et al.).
2. Try Ensemble methods. Combining your best models will often produce better performance than running them individually.
3. Once you are confident about your final model, measure its performance on the test set to estimate the generalization error.

## Backlinks
* [[§Machine Learning]]
	* [[Algorithm selection and design for ML]]

<!-- {BearID:E7112A66-E48A-48D7-804D-C1BFA9DAABB8-93658-0000017B2D2FC4C1} -->

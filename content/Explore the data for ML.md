# Explore the data for ML
Note: try to get insights from a field expert for these steps.
1. Create a copy of the data for exploration (sampling it down to a manageable size if necessary).
```
import pandas as pd
file_path = ".../.csv"
df = pd.read_csv(file_path)
# df_sampled = df.sample(n=X, random_state=42)
```

3. Create a Jupyter notebook to keep a record of your data exploration.

5. Study each attribute and its characteristics:
`data.head()`
`data.info()`
`data.describe()`
```
%matplotlib inline
import matplotlib.pyplot as plt
data.hist(bins=50, figsize=(20,15))
```
	1. Name
	2. Type (categorical, int/float, bounded/unbounded, text, structured, etc.)
	3. % of missing values
	4. Noisiness and type of noise (stochastic, outliers, rounding errors, etc.)
	5. Usefulness for the task
	6. Type of distribution (Gaussian, uniform, logarithmic, etc.)

1. For supervised learning tasks, identify the target attribute(s).

3. Visualize the data.
	1. Histogram for all variables
	2. (Box-plots by time for all variables)
	3. [[Pandas: Scatterplot]]

4. Study the correlations between attributes.

6. Study how you would solve the problem manually.

8. Identify the promising transformations you may want to apply.

10. Identify extra data that would be useful (go back to “Get the Data”).

12. Document what you have learned.

## Backlinks
* [[§Machine Learning]]
	* [[Explore the data for ML]]

<!-- {BearID:661FCF6E-DE2D-41BF-A9A8-B2265EC38ED8-93658-0000017A05AE7F93} -->

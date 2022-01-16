# Collect data for ML
Note: automate as much as possible so you can easily get fresh data.

1. List the data you need and how much you need.
2. Find and document where you can get that data
3. Check how much space it will take
4. Check legal obligations, and get authorization if necessary
5. Get access authorizations
6. Create a workspace (with enough storage space).
7. Get the data.
8. Convert the data to a format you can easily manipulate (without changing the data itself).
9. Ensure sensitive information is deleted or protected (e.g., anonymized).
10. Check the size and type of data (time series, sample, geographical, etc.).
11. Sample a test set, put it aside, and never look at it (no data snooping!)
	1. Random sampling
```
train_path = "/kaggle/input/home-data-for-ml-course/train.csv"

data = pd.read_csv(train_path)

from sklearn.model_selection import train_test_split

y = data.y-variable

X = data.drop('y-variable', axis=1)

train_X, val_X, train_y, val_y = train_test_split(X, y, random_state=1)
```
	2. Consider stratified sampling (if one variable is a strong predictor and you want to ensure it is is balanced between test and training set)

## Backlinks
* [[Algorithm selection and design for ML]]
	* Remember to use your validation set from [[Collect data for ML]].
* [[§Machine Learning]]
	* [[Collect data for ML]]


## Backlinks
* [[Algorithm selection and design for ML]]
	* Remember to use your validation set from [[Collect data for ML]].
* [[§Machine Learning]]
	* [[Collect data for ML]]


## Backlinks
* [[Algorithm selection and design for ML]]
	* Remember to use your validation set from [[Collect data for ML]].
* [[§Machine Learning]]
	* [[Collect data for ML]]


## Backlinks
* [[Algorithm selection and design for ML]]
	* Remember to use your validation set from [[Collect data for ML]].
* [[§Machine Learning]]
	* [[Collect data for ML]]

<!-- {BearID:51D3515D-34DB-4EC4-8815-11574EEE6341-93658-00000179AC79FECE} -->

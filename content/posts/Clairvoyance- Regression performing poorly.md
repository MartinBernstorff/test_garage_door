# Clairvoyance: Regression performing poorly?
To answer this, we need to be able to inspect the test-results. So far, I get an ndarray with shape 6, 3, 1. This is weird! I would expect one prediction pr. row in the test set. 

* Check the shape of the testing_dataset
	* As expected

* Oh, the time-units aren't whole numbers!
	* And the window-size must be integers?!
	* Adjust the dataset to be integer-based
		* Makes for faster training, but doesn't solve number of output predictions

* One way of getting around this is to try and do online classification instead.

<!-- {BearID:6E0A4A43-6C94-4E77-849A-6B3B4652AD10-63716-00000422DA6DE301} -->

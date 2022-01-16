# §Machine Learning
<!-- #anki/deck/ML# -->

* [[ML notation]]
* [[Anatomy of a Learning Algorithm]]
* Solving a problem
	* [[Frame the problem for the algorithm to solve]]
	* [[Collect data for ML]]
	* [[Explore the data for ML]]
	* [[Data cleaning for ML]]
	* [[Algorithm selection and design for ML]]
	* [[Present Your Solution for ML]]
	* [[Launch Your ML Model]]
* Basic algorithms
	* Regressors and classifies
		* [[Logistic regression]]
		* [[Decision tree learning]]
			* [[Random forest]]
		* [[Neural networks]]
			* 
	* Classifiers
		* [[Support Vector Machine (SVM)]]
		* [[k-Nearest Neighbours]]
	* Regressors
		* [[Linear regression]]
* Data management
	* [[Feature Engineering]]
	* [[Learning algorithm selection]]
		* [[Overfitting]]
	
* [[Data Leakage]]

---

Q. What does it mean for machine learning to be supervised?
A. Each example has a “true” label

Q. What does it mean for machine learning to be unsupervised?
A. The examples don’t have a “true” label

Q. What does it mean for machine learning to be semi-supervised?
A. The dataset contains both labeled and unlabelled data

Q. What is a feature vector in machine learning?
A. A collection of features describing the example

An epidemiological {variable} is in machine learning called {a feature}.

Q. What is the theoretical argument for model parsimony?
A. Avoid overfitting (ie. Occam’s razor) 

Q. Why do we care about the gradient of a function?
A. When gradient = 0, minimum or maximum has been achieved.

Q. What does a cost function express?
A. A function to minimise for regression

Q. What does it mean for machine learning to be batched?
A. Updating the model requires training on all the data

Q. What does it mean for machine learning to be online?
A. Updating the model requires only adding the new data

Q. How does batched learning differ from online learning in ML?
A. Batched requires re-training on all the data, online can re-train using only the new data.

<!-- {BearID:FB8B5C6C-F152-4307-A32D-C43DE0123298-4241-000007924D40E8D5} -->

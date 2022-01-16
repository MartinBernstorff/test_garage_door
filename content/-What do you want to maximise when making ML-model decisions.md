# ?What do you want to maximise when making ML-model decisions
* Number of patients that develop the outcome with at least one prediction
	* Maximises equity across patients, but probably not the most important.

* Total number of predictions/proportion of all visits in the dataset that we can make predictions for
	* Has a tendency to overweigh patients with many visits. However, is that so bad? 
		* It may cause more inequity, if some patients avoid the healthcare system
		* But it also may maximise the total benefit derived from the model. 
			* Benefit is derived from making correct predictions and acting on them. 
			* More correct predictions often leads to more correct actions – especially if we gap X months from "yes" predictions. 
			* The gapping also downplays the overweighting of patients with many contacts.

## Backlinks
* [[Model-design T2D]]
	* [[?What do you want to maximise when making ML-model decisions]]

<!-- #p1 -->

<!-- {BearID:AC40E202-3A1D-4E87-B74E-3F9BA131FF5B-14366-000002431862CEEF} -->

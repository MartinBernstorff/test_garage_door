# §PhD: Implementation of T2D prediction
In general, the point of prediction is early detection and thus prevention/earlier treatment.

Our risk model can help in two ways:
1. For patients not receiving antipsychotics, it can estimate HbA1c – if it exceeds a threshold, we might want to measure it
2. For all patients, even those where HbA1c is measured, it can predict whether HbA1c is going to exceed T2D-thresholds in the future
	1. This can help us focus preventive measures that decrease HbA1c-slopes, e.g. diet, exercise etc.
	2. [[What determines the slope of HbA1c in clinical populations?]]

For T2D, this means as early as possible. For feasibility, since we have 1-9 years of follow-up, we probably can’t do more than 2-3 years.
	* [[Can we use censored data for ML?]]
	* [[Can we predict time to incident diabetes]]

One of the largest papers, “The Diabetes Risk Score”, predicts diabetes within 5 years (yes/no). 
https://care.diabetesjournals.org/content/26/3/725

### Open questions
*When do we make predictions?*
As early as possible. Probably the day before the patient has a F2F-contact.

*Which consequences does it lead to?*
Increased preventive measures, e.g. dietary advice, changes in medication etc.

*Which variables do we need for that?*
To better answer this question, we might want access to the structured variables, sort them by how frequently they occur, and then choose the frequent ones that make sense. Or just choose all of them?

*How do we handle missing information on the “gold standard”, e.g. patients where HbA1c is never measured?* 
Probably just something we’ll have to live with. I.e. they’re labelled as negatives, but we might have “false negatives” in the labelled data.

*How do we define the outcome to be useful?*
By the most popular definition; ask physician. Add medications etc.
[[Udfaldsdefinition T2DBM]]

*How do we inspect data quality?*
	Box-plots by year for all structured variables
	Histograms for all structured variables

<!-- #p1 #service #sp -->

<!-- {BearID:87DF87A2-1A9E-44A9-ADDC-D478A224D745-93658-0000016DE60A1E38} -->

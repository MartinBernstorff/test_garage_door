# Danielsen review
/Predictive/counterfactually predictive/
Hvorfor justerer de for confoundere, når de ikke mener det er causal inference.

Strongly agree that you should not adjust for a descendant of the exposure that affects the outcome (e.g. a mediator) if you’re doing causal inference. 

“The variables that are adjusted for, were chosen as they are regarded as potential true confounders and hence not a consequence of the exposure.”

Why do you talk about confounders, if your study is not to be interpreted as causal inference?

“As hypothesized, maternal SMI resulted in higher IRRs of child psychiatric disorders than paternal SMI.”

Resulted in implies a causal pathway. 

/Comment 1: Were children censored from eg. “Injuries and poisoning”, “Fractures” and “Burn” after the first diagnosis? Given that a child can receive many diagnoses within these categories, even repeat incidence of the same diagnosis, does this lend itself to an intuitive interpretation of the incidence rates ratios? Ie., is “incidence of first fracture” a meaningful measure?/

/Re: the age-stratified analyses (table 2). If a child received a new diagnosis for eg. ”neurodevelopmental disorder” at 6 months old, was the child then excluded from the analysis of “1-3 year olds”? If so, how come that the time at risk for 1-3 year-olds is smaller than that of 4-6 year-olds? (151.121 vs. 159.967). If not, does this way of analyzing the data make sense – ie. does it make sense to censor a child in the at 6 months after receiving a diagnosis, but then re-enter them in the stratum for 1-3 year olds?/

Yes, a child with a diagnosis at 6 months is excluded from the analysis of the older age-groups. In order to use all data, we also use data from children without a full follow-up. This means that children of the latest year groups in the study are censored before they turn e.g. 5 or 6 years old. In this way, there are fewer person-years in the oldest age-groups, as individuals from the latest year- groups only contribute to the youngest age-groups. Hence, looking at number of person-years in each age-group does not convey the best picture, but incidence rates can be compared. The survival analysis (Poisson Regression which will give the same result as a Cox Regression) takes account of in- and out censoring.

Thank you for this clarification. 

If this is the case, I completely agree with the consequences the authors present, that there are *fewer* person-years in the oldest age-groups. 

However, this is not what I see in table 2. When comparing 1-3 y.o. with 4-6 y.o. of parents with SMI, there are more person-years at risk in the younger group every time (e.g. 151121 vs. 159967). 

I hypothesise that this is due to treating parental SMI as a time-varying covariate. If parental SMI has a higher incidence when the children are 4-6 years old, that would shift the risk time between the groups. If that’s the case, I have nothing further to add.

/All diagnoses for a given contact were counted./

I believe this to be quite relevant to the interpretation of outcomes, and would recommend that this is added to the paper. I would further recommend that the authors specify in which way contacts are categorised in table 3 – e.g. if a contact has an A-diagnosis of an infection, but a B-diagnosis of asthma, is it counted multiple times? Only for the A-diagnosis?

/However, previous studies generally indicate, that maternal mental health problems are positively associated with more problem-related child health-care visits /also among mothers outside the mental health care services/

Seems to have the same issue.

<!-- {BearID:5B8F1EBA-9480-423A-A280-B90A54825156-64154-0000CA861268BDBE} -->

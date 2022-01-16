# Advanced Methods in Pharmacoepidemiology
*Propensity scores*
Assumptions:
* Positivity – all units must be able to receive treatment (eg. no absolute indication or contraindications)
Probably more, haven’t been talked about. 

A multivariate model of being treated.
![](BearImages/D3007793-1E22-430A-941F-94B5569B076A-2458-000009C0032F79A0/9A1066F5-DBE7-4F34-8575-7B4432004BBE.png)

Typically used for matching or as a covariate, to adjust for confounding. 
* Matching 
* Stratification 
* Inverse treatment probability weighting (ITPW): As a weighting criterion (1/PS for treated, 1/(1-PS) for untreated), eg. The reciprocal value of the probability of receiving the treatment than you actually receive
	* ITPW: What if we treated everyone in the whole population, vs. treating none of them?
	* PS: What if we hadn’t treated those who actually got the treatment?

Can’t adjust for unmeasured confounding.
	* Nearest neighbour
	* Sequential, balanced nearest neighbor
	* Greedy

In the case of covariate imbalance (eg. Cohen’s d > .1):
* Include it in the adjustment along with the PS or
* (Up-weigh it in the regression model that builds the PS)

We typically trim the tails, to remove those with near-absolute indications and contraindications (since they don’t really provide much information to us – those are the ones we know need treatment, or know shouldn’t have treatment. If treatment is contrary to prediction, it means something weird is going on. Eg. some prediction to unmeasured confounding (“clinical despair”, “we have to do something, even though we break the guidelines”).

![](BearImages/504D7FB6-B8DB-4620-B8D7-73B0A6953985-2458-00000B21CD28F883/1453C83B-36D6-4889-93E7-11CFE0355D18.png)


![](BearImages/7105D734-7ACC-494D-9E49-44B8E6A42F9F-2458-00000B46047AD12D/23D3F17D-D761-421D-A485-847E0CEF34DF.png)

Risk factors for the outcome but not associated with exposure, means that we match based on everything associated with the outcome except the main exposure. Removes noise on both sides (eg. exposed and unexposed), essentially.

* What are the advantages compared to using those variables specifically?
	* Smaller confidence intervals?, but a loss of information?

* How does it fit into a causal understanding of confounding?
	* Eg. how do we avoid collider-bias or over-adjustment bias?


## Weighting
![](BearImages/7A913580-3E1D-4426-B2ED-24A352B24B37-2458-00000DBAD06A110F/64916320-DA4D-4A58-AA6D-1F030D9A393A.png)

<!-- {BearID:400D26FC-D345-4E40-B050-6A7FAEC5D1F7-2458-00000909ED8DC19F} -->

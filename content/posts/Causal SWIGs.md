# Causal SWIGs
Single world intervention graphs.

Q. What does [[§Exchangeability (Causal Inference)]] mean in causal inference?
A. We can use a treated person’s outcome as an untreated’s counterfactual

Q. Which biases must be absent for [[§Exchangeability (Causal Inference)]] to hold?
A. No confounding, unbalanced effect modification, measurement bias or selection bias

Q. How can we identify [[§Exchangeability (Causal Inference)]] in a DAG?
A. No open backdoor paths

Q. Why can we often only examine causal effects on populations, not individuals?
A. We can’t examine the counterfactual at the individual level; we can’t go back in time.

Q. 
![](BearImages/44BF906E-EB67-4980-B0AE-3B91DBB020EA-972-0000063ACDF84A7F/CFCC9723-FC45-4FA7-A962-406296409E38.png)
In causal inference, what is the meaning of the right side of the arrow?
A. The average outcome if all individuals had received treatment a = 1.

Q. 
![](BearImages/39458416-B839-492B-9C45-21A1829518BD-972-000006527F371381/CFCC9723-FC45-4FA7-A962-406296409E38.png)
In causal inference, what is the name of this type of graph?
A. SWIG - single world intervention graph

Q. Why might you use SWIGs instead of DAGs?
A. They make explicit which variables must be separated for exchangeability.

Q. 
![](BearImages/0A017AFD-5AB4-4EAA-95DF-B53167DDABD1-972-0000064907EC9F43/83766E07-BBD7-413A-AB3F-74C2CC9EC984.png)
What do we call this notation in causal inference?
A. Node splitting

Q. When are SWIGs preferable to DAGs?
A. In complex settings, eg. time-varying treatment

<!-- #anki/deck/Causal inference# -->

<!-- {BearID:2DACC899-5067-4182-AC36-FC0C1D58104B-972-000004847D6D407C} -->

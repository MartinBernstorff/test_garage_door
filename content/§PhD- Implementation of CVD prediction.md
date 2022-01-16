# §PhD: Implementation of CVD prediction
In general, the point of prediction is early detection and thus prevention/earlier treatment.

Treatments for cardiovascular diseases are either preventive (and typically directed at risk factors), etiological (and directed at the disease) or symptomatic.

[[Treatment modalities for CVD]]

Since the cost of treatment (resource-wise in the broadest sense; time, money, energy) varies dramatically, as does the benefit, cost/benefit trade-offs are going to vary dramatically too. 

This means that the value of prediction differs by outcome, and the timing probably depends on the disease as well as the available treatment. It is essentially a screening problem.

For most cases, earlier prediction is better. 

### Open questions
*What do we predict?*
[[Do we want to do multitask learning for CVD]]
[[Can we predict time to incident CVD]]

*Hjertet*
1. Akut iskæmi (AMI/CABG/PCI/trombektomi)
2. Kronisk iskæmi (ustabil angina, kronisk iskæmisk hjertesygdom)

*Hjernen*
1. Blødning
2. Iskæmi
3. Stroke UNS

[[Do we want to separate predictions into bleeds and clots]]

*When do we make predictions?*
We might want to imitate other prediction models, e.g. SCORE2. They try to predict a composite of CVD mortality, non-fatal MI and non-fatal stroke, and they do 10-year risks by different risk-strata. We probably can’t do 10-year risks (since our average follow-up is probably around 5 years), but maybe 2-3-year risk?

*Which consequences does it lead to?*
Collecting more information – [[Should predictions trigger collecting more information]]

Prevention – probably not direct treatment (ekko, KAG, Holter). Worth it to ask a cardiologist, though.

*Is that useful?*
[[Batched or incremental/live learning for ML-predictions]]

*Which variables do we need for that?*

[[Udfaldsdefinition CVD]]

---

[[When do we generate predictions for CVD]]













<!-- #p1 #service #sp -->

<!-- {BearID:51AB5192-274A-4577-AB4B-E72AE1B6210B-93658-0000016E0CED323A} -->

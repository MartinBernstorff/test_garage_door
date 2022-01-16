# How do we want to split the train, validate and test data
Advantage of slices across projects:
* We can re-use pre-training of models while maintaining pre-training <-> test-set independence

Disadvantages:
* We can’t do stratified sampling by the predictors we think to be most important for each individual outcome
* Test-set absolute size will vary due to exclusion criteria (i.e. don’t predict T2D in a patient that already has it)
* Test-set absolute size can’t be increased for rare outcomes that would otherwise contain few true positives

By slices I mean stratified sampling by:
1. Age (binned?)
2. Gender
3. Record year

Into:
1. Training set (80%) – which we also use for cross-validation
2. Validation set (10%)
3. Test set (10%)

## Next steps
- Write code – add it to utils?

<!-- #p1 #service -->

<!-- {BearID:94403C03-DFFB-4A4D-9AC1-C75A132FF40B-93658-00000185716CDBEA} -->

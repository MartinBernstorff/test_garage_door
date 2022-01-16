# Log: Clairvoyance tutorial
*03/01/2022*
* Look up Keras "online" predictions - maybe I can use that to get it to perform a prediction pr. time-period?
	* Rather than only one prediction in the end

---

* [[Clairvoyance: Regression performing poorly?]]
	* Can I get a look at those predictions?
* [[Clairvoyance: Classification performing poorly?]]

* When it says "outcomes" in temporal prediction, how does it predict them?
	* What is the meaning of "sequence length"?
	* The `window` setting is how far ahead it predicts! This might very well be the problem, I want it to predict the amount of sales *today*, not in the future
* Why is it performing poorly?
	* Check that outcomes match the ones I computed
	* Can we get the predictions out and compare them to the real number?
	* Can we do a correlation matrix?

<!-- #daily/2021/12/30 -->
---
`docker run -i -t -p 8888:8888 -v "/Users/au484925/Desktop/Clairvoyance introduction" clairvoyancedocker/clv`

For at kunne teste clairvoyance har jeg brug for et dataset der matcher. Dvs:

Prædiktioner om en enhed, hvor jeg har mange informationer om den enhed. Det kan f.eks. være prædiktioner om en butiks salg, hvor jeg bruger varekategoriernes salg som information om butikken.

Jeg kender ikke butikkernes samlede profit, men det kan jeg relativt hurtigt regne ud.

* train_test_split

* temporal_train_data
* static_train_data

* temporal_test_data
* static_test_data

<!-- #sp -->

<!-- {BearID:CAEB3A0E-78BC-4F1E-91A7-94B6ECB0FF9B-20566-0000005ACBC88087} -->

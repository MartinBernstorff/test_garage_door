# Long short-term memory (LSTM) net
Uses the [[Hyperbolic tangent function]], which is:
1. Centered around 0
2. Has a steeper slope than the [[Logistic function]]

Means we have stronger gradients, which:
1. Allow faster convergence
2. Don't disappear as quickly through iterations

An LSTM is a [[Recurrent neural net (RNN)]], which in each module has the following gates:
1. Forget gate, decides to which extent to use the previous hidden state
2. Input gate, to which extent to use the current input

For more: [Understanding LSTM Networks -- colah's blog](https://colah.github.io/posts/2015-08-Understanding-LSTMs/)

---

Q. Which type of neural net is the [[Long short-term memory (LSTM) net]]?
A. A gated [[Recurrent neural net (RNN)]]

## Backlinks
* [[Recurrent neural net (RNN)]]
	* To solve some of these, [[Long short-term memory (LSTM) net]].
* [[Long short-term memory (LSTM) net]]
	* Q. Which type of neural net is the [[Long short-term memory (LSTM) net]]?
* [[Neural networks]]
	* [[Long short-term memory (LSTM) net]]

<!-- #anki/deck/ML -->

<!-- {BearID:72261739-28FC-4878-8C97-396C2AA5B037-43256-0000017C4997A370} -->

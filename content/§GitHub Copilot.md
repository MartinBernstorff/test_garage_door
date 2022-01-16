# §GitHub Copilot
Probably mostly pretty useful. It is so much easier to identify and test a decent suggestion than it is to create one yourself. It helps you to get to "good enough" as fast as possible.

For larger projects, the bar for "good enough" is probably a lot higher! Most of the time is spent debugging and writing tests; this means that code that is poorly factored is a *lot* worse. 

Helps tremendously with:
* Template code
* Solving moderately difficult problems
* Getting basic functions to work

Some issues:
* Prompts regression towards the mean because it is only as good as the average programmer
	* Doesn't know which functions are already implemented in the language, might create duplicate functions
	* Often suggests code that is
		* Verbose
		* Not refactored

* Removes important feedback loops that are present with e.g. Stack Overflow. 
	* Human-generated examples get the advantages of humans; they consider context. And, even more importantly, they're often weighted by quality! This avoids regression towards the mean, but moves us all upwards faster!
	* Highly likely to use old syntax
	* Doesn't think about edge cases
	* Assumes that you approach (e.g. "use regex") is the correct one

* [[Automation Bias]] and [[Anchoring Bias]]  mean that we might follow copilot's path too often. 

Will I use it for the ML PhD, then? Depends on whether the type of things I will be doing will benefit from it – will they?

## References
[[Is GitHub Copilot a blessing, or a curse? · fast.ai]]

<!-- {BearID:AF1B5195-5BD8-46DC-A8C1-9D671F83F8F0-8349-0000051C77549DA3} -->

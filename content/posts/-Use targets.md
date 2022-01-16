# ?Use targets
Current pain points:
* Unsure about whether dependencies have changed before outputting a file
	* I can just knit it when outputting – does require a lot of time, though
	* Functions
		* Can I run a field (e.g. source functions) whenever any field is run? 

	* Data currently in environment
		* I can cache when knitting!
			* https://bookdown.org/yihui/rmarkdown-cookbook/cache.html
			* This caches the output of a code-chunk dependent on that chunk – i.e. it doesn’t check if previous chunks have been modified
			* It also doesn't help with updating data in the environment
		* Can I get more speed using dbplyr?
		* Or by asking Bettina?

Can be solved by knitting, but results in long wait times as preprocessing is repeated.

*Downsides about implementing targets*
* Decreased readability for collaborators
* ?Might make debugging harder

But doesn't solve:
* Not certain about whether underlying data or functions have changed when knitting

## Backlinks
* [[12/11/2021 - Work]]
	* [[?Use targets]]
	* ?Implement targets – see [[?Use targets]]

<!-- {BearID:611DCF93-DC48-4C1B-A26D-BB69AB379751-19673-00000661E0DEBF8C} -->

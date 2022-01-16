# Gittins index
For an [[Explore or Exploit problem]] where the future is infinite, but wins are future-discounted geometrically:

$$ v = v_{0} · (1-d^{t}) $$

Where d is the discount rate and t is the number of trials.

You calculate the Gittins index for each option, and then choose that option.

Assuming 10% discounting pr. trial:
![[Attachments/Pasted image.png]]

Assuming 1% discounting pr. trial:
![[Pasted image 1.png]]

This shows that the lower the discounting, the more we should explore.

## Backlinks
* [[Explore or Exploit problem]]
	* For an exact solution, look at the [[Gittins index]].
* [[Upper Confidence Bound Algorithm]]
	* Pick the option with the highest upper confidence bound. Similar to the [[Gittins index]], but don't require future discounting and are much easier to compute.
* [[Can I use multi-armed bandit problem for time well spent?]]
	* I can! E,g. use a [[Gittins index]] calculated from the last x days.

<!-- #Life -->

<!-- {BearID:B2E43B69-CB0B-4704-A663-61AA0AF9E94A-15756-0000130367D87CA7} -->

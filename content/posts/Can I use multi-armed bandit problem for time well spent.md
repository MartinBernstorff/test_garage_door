# Can I use multi-armed bandit problem for time well spent?
[[$My Implementation of Life Well Spent (LWS)]]

I can! E,g. use a [[Gittins index]] calculated from the last x days.

Turns out Gittins indexes are pretty hard to compute. Might instead use an [[Upper Confidence Bound Algorithm]], Eg. calculate some interval estimating confidence, and then order the options by their upper bound.

To do this, I want to:
+ Estimate variance
	+ Avg. rating
	+ Calculate deviation for each item
	+ Use those to calculate SD
+ Use variance to estimate upper bound
+ Set a standard variance for first observation

<!-- {BearID:2AED9F39-719F-4593-B4EC-41440EE4D0B4-945-000004B852CAA0DA} -->

# §Sorting
Sorting, in the general case, is helpful to reduce look-up times.

In more specific cases, it might help with:
* Social norms
	* Aesthetics
* [[Peripheral vision (design)]], knowing that you even had the item

The optimal sorting algorithm, if you don’t know anything about the distribution, is [[Merge sort]], which hits O(n^2).

And if you do know something about the distribution of items, [[Bucket sort]], which hits O(n · m), where m is the number of buckets. Choosing the right buckets here is essential, and depends on [[§Forecasting]]. 

In real life, though, since there are linear costs to physically moving things around, the [[§Insertion Sort]] can do pretty well, too.

## Backlinks
* [[§Caching]]
	* Another way of speeding up access-times is [[§Sorting]], where the cost is compute.
	* How, then, do you know whether [[§Sorting]] or [[§Caching]] is the right thing to do? Depends on the cost - is compute more expensive than memory?
* [[§Selection]]
	* This reduces it to a [[§Sorting]] problem.

<!-- {BearID:BC51097A-9CBF-4D77-A66C-6EFA363FFA07-7797-00000A275ED23366} -->

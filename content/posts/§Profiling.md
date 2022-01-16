# §Profiling
---

Q. You're working on a dataset where the code takes more than 30 seconds to run. What is the most efficient way of improving its performance?
A. 1) Slice the dataset, 2) Profile the slice, 3) Improve. Keep going until good enough. Try again with larger slice (to look for things that scale non-linearly).

Q. How much should you optimise the speed of your code?
A. As little as possible, but as much as required.

Q. Which criteria must code fulfil to be "fast enough"?
A. 1) Cost-effective iteration time in dev, 2) Fast enough runtimes on implementation, 3) Not cost-effective to save compute

[[?Time track to improve your life]]

[[Do I want to switch to Bear]](bear://x-callback-url/open-note?id=4B0A5E65-B57D-48EE-B2A7-1B8AEBB3B681-2532-0000087024D3EA93&show_window=yes&new_window=yes)

## Backlinks
* [[?Time track to improve your life]]
	* Assuming time-tracking is supposed to lead to efficiency improvements, like [[§Profiling]], when does it make sense to time-track?
* [[27/10/2021 - Work]]
	* Time spent [[§Profiling]]

<!-- #anki/deck/Programming -->

<!-- {BearID:1336DF52-56AB-4E67-8FCB-2B5CB1B07688-43256-00000169B8D5A99F} -->

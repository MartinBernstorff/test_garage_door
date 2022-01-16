# §Scheduling algorithms for a single agent
*Throughput*
* [[Impact Density Scheduling]]: Do the task with the highest impact density (effect / duration) first. 

*Calendar time ([[§Deadlines]])*
* [[Minimise lateness]]: We do tasks in the order of due date.

* Minimise number of items late - [[Moore’s algorithm]]. Do tasks in order of due date. If the next item is going to pass its due date, look forward and drop the largest item (to gain the maximum buffer for the minimum cost).

[[Minimise lag time]], [[Close open loops]]
* [[Shortest Processing Time]]: Do the smallest projects first. 

[[§Procrastination]] can be seen as a strategy to [[Close open loops]] – you do the small tasks first, so you can get them off your mind. Another, better method is probably to just let the task be, if it isn’t ever going to the top of [[Impact Density Scheduling]] - either through pure density or [[Priority inheritance]]

## Backlinks
* [[§Scheduling for a single agent]]
	* Which algorithm is optimal depends on which metric matters most to you, albeit its typically a trade-off between [[Throughput]] and [[Responsiveness]]: [[§Scheduling algorithms for a single agent]].

<!-- {BearID:44DF1672-BB18-4D95-860F-B079EA4847AC-4122-000006093ED77D04} -->

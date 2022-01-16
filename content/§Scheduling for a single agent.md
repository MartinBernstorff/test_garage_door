# §Scheduling for a single agent
If you have only a single machine, and you will do all of the tasks, the order can’t affect the total completion time (except for efficiency considerations, see below).

This makes [[§Prioritisation]] more important than sceduling.

Which algorithm is optimal depends on which metric matters most to you, albeit its typically a trade-off between [[Throughput]] and [[Responsiveness]]: [[§Scheduling algorithms for a single agent]].

My synthesis is here: [[§How I schedule tasks]].

Moderately complicated scheduling problems are often intractable, unless we allow for [[Preemption]] - the ability to stop a task mid-way through and switch to another. This returns [[Impact Density Scheduling]] to the top – if you get another option, and it’s better than the current one, simply switch to that. 

Turns out this problem is intractable if you know both starting dates and durations – so it’s best to just ignore them?!

However, this is costly due to [[§Context Switching]] ([[Balance context switching]]). When, then, should we switch? I think when the increase in impact (time · density) is larger than the cost of the context-switch. Can we make that into a heuristic?

Worst case is [[Thrashing (scheduling)]].

*Efficiency considerations*
* [[§Batching]]
	* An example of [[Interrupt Coalescing (use Batching)]], to decrease [[§Context Switching]].

* [[JIT vs. JIC]]

* [[Zeigarnik Effect]] - probably not real.

* Dependencies
	* [[Priority inheritance]] - if a task is low-priority, but required for a higher-importance task to get done, it should inherit the importance of that task. E.g. if you need to clean your room to have your friends over, cleaning your room becomes high priority! This is essentially what we mean when something is instrumental ([[Instrumental Values]]).

Proposed heuristics:
* Eat That Frog: Hardest things first.
* GTD: < 2 min, do now. 
* Eisenhower Matrix: Important things first.

[[Round robin scheduling]]
A fixed time unit pr. process, then rotate between processes. Ensures all processes get some time. Similar to having e.g. “reflection” in the morning. Might be useful in that it leaves space for novelty-based exploration, like [[§Incremental thinking]]. 

Downsides is that it increases average waiting time, and total throughput is lower due to [[§Context Switching]]. 

For humans, throughput might be slightly higher due to [[§Incubation]] and [[§Reflection]] leading to strategy improvements. Also aids long-term memory, which might be both desirable and undesirable.

[[Multilevel feedback queue]]

## Backlinks
* [[§Prioritisation]]
	* What to do first? [[§Scheduling]], [[§Scheduling for a single agent]]
* [[§Scheduling]]
	* [[§Scheduling for a single agent]]
* [[11-Dec-21 - Homely]]
	* [[§Scheduling for a single agent]]

<!-- {BearID:9EEF0306-323A-413E-92B6-5A2C6A379DD0-3179-000004E4C5284019} -->

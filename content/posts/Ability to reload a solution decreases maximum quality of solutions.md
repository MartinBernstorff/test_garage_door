# Ability to reload a solution decreases maximum quality of solutions
From [[Bernstein 2018]], shows that if we’re looking to find the optimum solution, ability to refer to previous solutions is not necessarily a good idea. However, in real-world scenarios we often want to [[Increase reusability]] because the solutions we have are adequate. Furthermore, speed is often way more important than finding the optimal solution – eg. producing a computer is way more important than finding the best way of producing a computer. Collaboration and storage work way better for speed, [[Collaboration speeds up problem solving]].

Hmm, Bernstein seems to show the previous solution in the bottom left! 

> In rounds 2–17, subjects could see the solution they entered in the previous round, in a smaller window below the main task window, along with its distance.

> In the storage condition, subjects had an image corresponding to their own previous best solution, along with its distance, in addition to infor- mation about their own previous solution and information about their neighbors’ solutions, if applicable. Subjects could load their previous best solution by clicking on it. After loading, subjects could edit it or simply submit it as is.


This means all groups stored the last solution, and “storage” means storing the best solution – unless what they describe is only for the storage group.

Furthermore, [[Bernstein 2018]] shows that this is the case if we’re interested in finding the global optimum – but the o

Does this apply for novelty search as well? Probably not, since the previous trial doesn’t lead to the next novel attempt – rather, it excludes certain attempts from being novel.


This collides with [[Exploration is more efficient with memory]] – can I reconcile that difference?

### Objective vs novelty search
One potential reconciliation is that what Bernstein is talking about is an objective based search, in which case you can run into deception. If you reload solutions based on their performance, ability to reload reinforces deception.

Another is that [[Bernstein 2018]] only allowed recollection of the previous best solution, which would lead you straight to the local optimum. If they had instead allowed recollection of any previous solution, you could avoid creating the same solution multiple times, or iterate from one point.

This requires that you have a good map of the problem space though – either that you can identify which intermittent solution is most promising and work from that, or that you have multi-step paths leading to dead ends, ie. that the problem space has gaps where you can’t travel. Then you can easily identify if you’re going down a path that will terminate in a dead end, and turn around.

### How civilisations progress
Another parallel can be drawn to how civilisations advance – they tend to advance by building on each other’s solutions and knowledge. But [[Bernstein 2018]] didn’t test problems where partial solutions can be combined.

### Novelty search works for metric-less exploration
Much of what novelty search is thinking of is not objective based search, it’s a combination of ideas that result in solutions on a completely different metric, eg. transistors and computers.

Exploration in the broad sense is not objective based, it isn’t optimised by some performance metric. Rather, it optimises on novelty – and you cannot know if your approach is novel if you can’t remember previous trials.

## Backlinks
* [[Increase reusability]]
	* Why? Because it decreases time spent solving the same problem. This may decrease the probability of finding the optimal solution ([[Ability to reload a solution decreases maximum quality of solutions]]), but it does so while giving the benefits of dramatically decreased time spent exploring the problem space – and exploring the same part of the problem space.
* [[Problem solving in teams]]
	* [[Ability to reload a solution decreases maximum quality of solutions]]

<!-- {BearID:839054D4-F18A-447D-A0A0-F73E49A21D57-32756-0000335F919FEF66} -->

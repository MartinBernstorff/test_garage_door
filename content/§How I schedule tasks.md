# §How I schedule tasks
I do a combination of [[Just in time (JIT)]] and [[Impact Density Scheduling]].

I want to maximise my total throughput. This means [[Impact Density Scheduling]], with an adjustment for [[Neutral hour]]. 

Q. When is it efficient to preemptively context-switch?
A. When `∆Impact · Time > Context-Switch Cost`

## Backlinks
* [[§Scheduling for a single agent]]
	* My synthesis is here: [[§How I schedule tasks]].

<!-- #p1 What is the typical [[Typical Context Switching Cost]]? -->

For things that don’t realise their impact before a deadline, I wait until ~1.5x the expected completion time to start it. This minimises [[Carrying costs]] through [[Just in time (JIT)]] principles.

This seems to be what we do most of the time naturally, so scheduling through intuition is pretty good!

*Open questions*
* How do I trade-off with [[§Batching]]?

<!-- {BearID:E4BAF65C-0191-4E7D-819E-A90F2359975E-4122-0000060A3675E642} -->

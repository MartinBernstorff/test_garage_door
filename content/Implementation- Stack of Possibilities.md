# Implementation: Stack of Possibilities

### Basics
One outline might be a #project tag, with notes in Bear. On my computer, I can then just search for #project with the Alfred extension. On my iPad, this is possible too! Holy crap! 

### Weekly and monthly
I might use this for longer-term planning too, e.g. having a hashtag for each week and month which I can search in using the Alfred extension and “bw” and “bm”. This could expand pretty well, while maintaining high flexibility! [[§Weekly planning]], [[§Monthly planning]]. 

Might want to adopt a b `w[ork]|h[ome]``unit` `p[revious]|c[urrent]|n[ext]` syntax, with “days” being the base. So `bwc` for today’s work note, `bwwn` for next week’s work note etc.

For hashtags, something like `ww-yy` for weeks and `jan-21` for months. 

### Implementation
I fear the above implementation branches too much, making it difficult to find things when I want to! Granted, forced reminders isn’t what I’m looking for, but registering the same information at many levels isn’t either! 

One way around that is to:
	* Mostly link to project-notes, rather than write a lot in each period-note
	* Go through the relevant notes (e.g. weeks) when planning months.
	* Really, the organic way of doing this is probably the best! After all, [[Plans are useless, but planning is indispensable]].


* Decide on format
	* Start with day, month and year
		* Day, 5 Dec 2021
		* Month, `dec-21`
		* Year, `2021`
* Make Bear integrations
	- Can I do it programmatically?
		- E.g. `bh` and then parse the following characters
	- Add support for tags

<!-- #home/project #service/project -->

<!-- {BearID:2AB50945-96EC-4270-831F-1BF808C045C5-21973-000004E6DB4601D1} -->

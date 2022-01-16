# ?Retrieval prompts should include (only) the context available at usage time
To avoid overfitting, i.e. learning the card rather than learning the knowledge.

When we say information here, we mean it in the sense of [[§Information Theory]]. E.g. cloze-deletions typically include a ton of information, because you’re mapping to the combination of words, which is relatively unique. OTOH, even relatively long QA prompts can include low amounts of overfit-worthy information, if you’re not mentioning things that are idiosyncratic to the card.

More context makes it easier to match to a use-case, more likely for the memory to show up organically as you need it. 
But it also makes you prone to overfit – rather than creating a broad concept which applies within a certain set of parameters, you train for the test.

Less context makes the prompts harder, and makes you prone to misapplication (because its limits were underspecified), not applying the concept (because it isn’t prompted by the situation it might be useful in), and forgetting the concept (because you never apply it).

This seems related to [[Work at the right level of abstraction]].

## Backlinks
* [[?Use cloze-deletions to learn sets and lists]]
	* The big question is whether I’ll “overfit”; I must keep the prompts as short as possible (to give only context that’ll be available at the time I’ll need the information), but as long as necessary ([[?Retrieval prompts should include (only) the context available at usage time]]).
* [[Retrieval prompts should discourage shallow pattern matching]]
	* [[?Retrieval prompts should include (only) the context available at usage time]].
* [[Cloze deletion prompts seem to produce less understanding than question-answer pairs in spaced repetition memory systems]]
	* Cloze deletions typically include so much context that they allow for pattern matching/overfitting. This is less true if all it includes is a diagnosis and the items that are important to remember. It might also be possible to circumvent, at least somewhat, [[?Retrieval prompts should include (only) the context available at usage time]].
* [[Retrieval prompts should prepare you for a future situation]]
	* In this sense, this prompt is true. Cards are most powerful when they’re shaped so that they empower your future self This means that [[?Retrieval prompts should include (only) the context available at usage time]].
* [[§Qualities of good retrieval practice prompts]]
	* One argument for allowing [[?Retrieval prompts should include (only) the context available at usage time]] to be downplayed is that we allow the brain to make these connections. It's all about transfer learning, though, [[Practice how you play]]
* [[§Retrieval Practice (Qualities of a Good Practice)]]
	* [[?Retrieval prompts should include (only) the context available at usage time]]
* [[06/11/2021 - Home]]
	* [[?Retrieval prompts should include (only) the context available at usage time]]
* [[Examples can act as unit tests]]
	* [[?Retrieval prompts should include (only) the context available at usage time]]

<!-- #p0 -->

<!-- {BearID:D0FEA2A1-B692-485E-AE77-F3C156B19B77-471-000000D0173F157D} -->

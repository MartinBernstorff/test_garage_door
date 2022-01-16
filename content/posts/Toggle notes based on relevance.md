# Toggle notes based on relevance
The use-case is selecting which notes to keep repeating and which not as my semester ends, and as I switch between departments at the hospital. 

+ I typically want that to be done at the field x detail level, eg. I only want to retain paediatrics at an "akutmodtagelsen" level right now. 
	+ The process is not idempotent. Why is that?
	+ Check for #anki/deck tags in note
		+ Use those tags to select subdeck
	+ Match QX subtypes
		+ Use to set subdeck
		* It appears that changing the subdeck of the generated card doesn't move an already existing card in Anki. 
		* This means that my subdeck-moving mechanism won't work
			* Are there other things I can try to move cards?
			* Can I use another mechanism? Eg. add tags to cards via the same code, and then manually suspend/unsuspend
				+ Can this happen?
				+ Is it reversible (eg. will re-importing remove tags?)
	+ Match #anki/tag/med/specialty tags
		+ Use to set tags
		+ test.md (eg. akut myeloid leukæmi) genererer ikke kort
			+ It's due to the subdeck processing, somehow it fails

* One way of doing that is in Anki – generate a new deck for each level of detail beneath each specialty. But genanki handles multiple decks poorly (at least so Ankdown says), so that may not be a great solution. However, I haven't tested it myself, and it seems to fit the bill for all my needs right now.
* Another is to let each card inherit the tags of the note. This means that I can manually adjust rather easily from anki – but it also means that changing level of detail in the note isn't automatically applied.

+ Sometimes I want to disable a note or an entire category as well. 
* I think looking for #anki/tag/disabled, but the tag having to include only anki and disabled (eg. also works) is a good fit.
* Will have to move to a disabled subdeck, rather than not produce the card (to update old cards)

Dimensions:
Level of detail: GP, akut, hospital, eksamen. Are these mutually exclusive?

Use QG, QA, QH, QE prompts.

Specialty: #anki/tag/med/Hematology

Some entire cards can nicely be disabled, implement #anki/tag/disabled

How do I move a sub-category of cards? Eg. the hospital cards for paediatrics.

## Backlinks
* [[Make my personal mnemonic medium ready for medicine]]
	* [[Toggle notes based on relevance]]

<!-- {BearID:B2C06C5B-10F8-4E54-BDBC-1B88C0B729C4-1056-000001DDEDD50948} -->

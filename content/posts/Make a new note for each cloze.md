# Make a new note for each cloze
[[$My Personal Mnemonic Medium (instance)]]

What if I make a new note for each cloze? Then I can use
the cloze content hash + filename as the note ID.

Cards that contain the cloze as part of their context will still be updated, since they're regenerated on each r
un of the script.

I'll run into problems:
* I modify a cloze prompt, the old note isn't modified nor deleted.
	* Previously (when using hashing from filename with all clozes in the same note), each md resulted in only one note.
		* When I updated the files, the old cloze prompt number was overridden. This means that a modified cloze resulted in a new card and an empty card.
	* I can in find these new orphan notes in Anki based on "edited" time – this catches cards where the deck name has changed as well!

<!-- #Life -->

<!-- {BearID:666F9F9B-DD55-4B15-90A3-8CFEE1288973-15756-000013040889022A} -->

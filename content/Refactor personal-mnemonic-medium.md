# Refactor personal-mnemonic-medium
Right now I go line-by-line. This has a couple of problems:
	1. Makes it harder to write function-by-function tests, as it joins at compilation time

I’m suggesting a major refactor, that’ll probably make the code easier to read as well. Instead of going line by line, we’ll process the entire string at once.

# Major
Split into blocks first, then you can process those blocks as you see fit. This solves the multi-newline problem.

## Q/A
Questions start with “Q. “ and end when an “A. “ appears
Answers start with “A. “ and end when a double-newline appears.

::Q. `/(?:(?!A\. ).)*/s`::

* How will I match them? I can create lists, but that isn’t resistant to e.g. “QD.” when I temporarily disable a card. Then I’ll have to add a D to both Q and A. That’s doable.
	As an error-checking mechanism, check if len(Q) == len(A), otherwise raise a valueError.

## Cloze
Divide the text into blocks separated by 2 newlines.

For each block, check if there are clozes. If there are, generate cards.

# Minor
* Set model when initialising a card object.

<!-- {BearID:CABCCE55-4497-4706-8780-594CB0AEA079-36407-000000C4FD15D408} -->

# §Test driven development (TDD)
The idea to [[Quality check at low value]]. It’s a way of scaffolding [[§Informational feedback]].

Books: [[TDD by Gorman]].

Proposed consequences:
* Simpler code, becuase it is easier to test 
	* More flexible code, because simple code is easier to modify

* Better designed code, because you consider good interfaces when writing the tests

* Refactor more easily, because you’re confident your code will keep working

* More fun development cycles because of the rapid feedback

* Software is less costly to create, because you catch bugs and differences in requiements/expectations early ([[Quality check at low value]]). Known as defect prevention.

[[Plan from examples]]

*Princples*
* Don’t write source code until a test requires it
 
* Reference new classes, methods, functions etc. in your tests first, then write code that uses it

* Aim to have just one thing broken at a time, if possible

———————

Q. What indicates you’re writing too many tests?
A. You encounter bugs much below the acceptable rate for the project.

Q. What indicates you’re writing too few tests?
A. You encounter bugs that take longer to debug than the test would’ve taken to write, or at a rate above what is acceptable for the projects

Q. Which error in your markdown to anki workflow would [[§Test driven development (TDD)]] have prevented?
A. Change in hashing function -> losing scheduling information for thousands of cards.

## Backlinks
* [[§Test driven development (TDD)]]
	* Q. Which error in your markdown to anki workflow would [[§Test driven development (TDD)]] have prevented?
* [[How to Improve Your Productivity as a Working Programmer - malisper.me]]
	* Consider setting up [[§Test driven development (TDD)]] in R - especially for larger functions, allows to test and refactor them rapidly, without having to wait for long code-runs or modifying the markdown files. [[Unit testing \/ test driven development \/ TDD in R]] #painpoint
* [[20/11/2021 - Home]]
	* Read up on [[§Test driven development (TDD)]]
* [[A Philosophy of Software Design by John Ousterhout]]
	* How does he critique [[§Test driven development (TDD)]]?
* [[Do we want to use test-driven development?]]
	* [[§Test driven development (TDD)]]
* [[Extreme Programming Pocket Guide by chromatic]]
	* *Adopt [[§Test driven development (TDD)]].*
* [[The utility of testing increases as code runs take longer]]
	* [[§Test driven development (TDD)]]

<!-- {BearID:E5E5C8EB-F0F2-4D4A-A161-CDED0E47EDDC-37213-000003245B94F1CF} -->

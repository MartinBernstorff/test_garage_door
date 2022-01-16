# dplyr
Q. In dplyr, how might you apply a function to all columns that match a regex rule?
A. `mutate(across(matches(REGEX), ~ function(.x)))`

<!-- #anki/tag/R #anki/deck/Programming -->

<!-- {BearID:09FD6A40-2FD9-4B58-BB34-E30B80C0C6A9-8349-00000518A847E3B2} -->

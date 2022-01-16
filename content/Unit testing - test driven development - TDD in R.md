# Unit testing / test driven development / TDD in R 
https://rstudio-pubs-static.s3.amazonaws.com/278724_4d8935a2955c49d9934e2113c737e70e.html

See also chat with Ludvig Olsen, 09/12/2021 10:31.
### Setup
```
library("pacman")

p_load(testthat, here, datapasta)

source(here("src", "functions.r")

context("make_filename tests")
```

### Writing tests
* Use `p_load(datapasta)` to install.

* Source on save to run the tests when saving the tests file

Q. Which function outputs a hard-coded version of a data frame to the terminal in R?
A. `dpasta(df)`

### Modifying functions
`auto_test(here("src"), here("tests"))`

```
library("pacman")

p_load(testthat, here, datapasta)

source(here("src", "functions.r")

context("make_filename tests")

test_that("make_filename returns expected filename when passing year as integer",{
  expect_match("accident_2017.csv.bz2", make_filename(2017))
})

test_that("make_filename returns expected filename when passing year as character",{
  expect_match("accident_2013.csv.bz2", make_filename("2013"))
})
```

<!-- #anki/deck/Programming -->

<!-- {BearID:DF0EBBD0-FB91-4416-AB70-0F85BAC28C3B-3179-000004421541B35C} -->

# R docstrings (ROxygen)
Q. What does the equivalent of a "docstring" look like in R?
A. 
```
<!-- #' Add together two numbers -->
<!-- #' -->
<!-- #' @param x A number -->
<!-- #' @param y A number -->
<!-- #' @return The sum of \code{x} and \code{y} -->
<!-- #' @examples -->
<!-- #' add(1, 1) -->
<!-- #' add(10, 1) -->
add <- function(x, y) {
  x + y
}
```

<!-- {BearID:DBA47333-C99D-4274-8BCE-58DD75627882-2970-000002ED93775A88} -->

# R introduction
<!-- #anki/deck/Programming #anki/tag/R -->

Q. How do you define a variable in R?
A. 
```r
myvar <- valueOfMyvar
```

Q. How do you supply arguments to a function in R?
A. 
```r
myFunc(argument_value)
```

Q. How do you list available variables in R?
A. 
```r
ls()
```

Q. How do you define a container-vector in R?
A. 
```r
p <- c(2,3,5,7)
```

Q. 
```r
p <- c(2,3,5,7)
```
What is `p[3]` equal to in R?
A. 5

Q. What is `p[-3]` equal to in R?
```r
p <- c(2,3,5,7)
```
A. 
```r
p <- c(2,3,7)
```

Q. How do you convert to an int in R?
A. 
```r
p <- c(2,3,7)
p_int <- as.integer(p)
```

Q. How do you define a function in R?
A. 
```r
sum <- function(a, b) {
    return (a+b)
}

sum(2, 3)
```

Q. How do you call sum in R?
```r
sum <- function(a, b) {
    return (a+b)
}
```
A. 
```
sum(2, 3)
```


Q. How do you iterate over a vector in R?
A. 
```r
for (item in vector_name) {
	# do things...
}
```

<!-- {BearID:127EF092-15C5-4E6E-ADAC-666B5554C424-640-00000F20CFF60CA9} -->

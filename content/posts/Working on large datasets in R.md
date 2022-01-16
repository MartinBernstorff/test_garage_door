# Working on large datasets in R
1. Do development on a subset of the data
2. Use dtplyr, or if necessary, parallelism: [A Multi-Process dplyr Backend • multidplyr](https://multidplyr.tidyverse.org/index.html)

Q. How might you select 10% of a dataframe in dplyr?
A. `df %>% slice_sample(prop=0.1)`

Q. How might you speed up debugging on large datasets?
A. 1) Unit-testing, 2) Sample a proportion of the dataset from the step right before the step you're debugging, 3) Cache the data (.csv or similar) 

Q. You're waiting a long time on data-processing so you can modify a plot. How might you save time?
A. Save the preprocessed data as a .csv

Q. You're waiting on a process in R. There is no way to speed it up. How else might you save time?
A. 
```r
library(future)
plan(multiprocess)

output %<-% slow_function()
```

## Backlinks
* [[15-Dec-21 - Work]]
	* [[Working on large datasets in R]]

<!-- #anki/tag/R #anki/deck/Programming -->

<!-- {BearID:48AA0A59-75A8-45F7-95A4-5B474682FA63-8815-00000015BC7715F5} -->

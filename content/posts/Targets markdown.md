# Targets markdown
```{targets globals, tar_globals = TRUE, tar_interactive = TRUE}
options(tidyverse.quiet = TRUE)

tar_option_set(packages = c("biglm", "dplyr", "ggplot2", "readr", "tidyr"))

create_plot <- function(data) {
  ggplot(data) +
    geom_histogram(aes(x = Ozone), bins = 12) +
    theme_gray(24)
}
```

A chunk takes the form:
``` {targets chunk_name}
list(	
	tar_target(return_element, function)
)
```

Typically you'll write the function separately. If you want to define the function in the Rmd, you can do:
```{targets chunk_name, tar_simple = TRUE}
data <- data
biglm(Ozone ~ Wind + Temp, analysis_data)
```

This works as long as the function returns only one value.

It then automatically runs tar_target around it. All other options for tar_target are default, but can be modified with tar_option_set in a tar_globals chunk.

When you're ready to stop running things manually, you want to run in non-interactive mode. This happens when you knit/render the whole document.

* How does it handle avoiding renewed SQL pulls?

* Right now I can do knitr to run in non-interactive, but then I can't do tar_visnetwork(). 

If you want to set some options differently based on whether you're running in interactive or non-interactive mode, you can use:
`tar_toggle(interactive_option, non_interactive option`. This is advantageous in that you can keep the interactive runs short, while keeping the full runs detailed.

*Workflow 1*
1. Change `tar_interactive` to `FALSE`
2. Run all chunks to update their non-interactive counterparts

4. Run a `tar_visnetwork()` R block
5. Run a `tar_make()` R block

To inspect results, do `tar_read(object_name)`

* I'm unsure how this handles the SQL calls

*Workflow 2*
My ideal is to be able to run the make command every time I make changes, and then see the output within an interactive session. 

What I can do, though, is to run
`tar_make()` in RStudio on the server, and modify functions via VSCode. This should be more pleasant.

## Debugging in targets
To get error messages:
```
tar_meta(fields = error, complete_only = TRUE)

tar_meta(fields = warnings, complete_only = TRUE)
```

## Backlinks
* [[Targets (R)]]
	* [[Targets markdown]]

<!-- {BearID:E329C0BE-D0ED-412F-921D-1977136384D6-931-000000122E26F48A} -->

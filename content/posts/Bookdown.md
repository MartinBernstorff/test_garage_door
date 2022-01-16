# Bookdown
A tool to generate rmarkdown reports in [[RStudio]].

The way I use it is:

* Put all markdown files in an Rmd folder. Each file must:
	* Have one top-level h1 
	* No other H1s

* Create a "render".rmd file in the top-level folder with: 
```
library("bookdown")
library("here")

bookdown::render_book(input = here("rmd"))
```

* Add a bookdown.yml containing:
```
rmd_subdir: ["subchapter_props/", "individual_unique_diagnoses/", "stability_connected_series/"]
delete_merged_file: TRUE
```

<!-- {BearID:6CB8FF77-D362-4AE5-8CC0-169DD6A40682-92688-0000067631D98B73} -->

# vignettebuild

The goal of vignettebuild is to try to illuminate some confusion/difficulty I am having getting `.Rbuildignore` to do what I want.

There are three interesting files in this repository:

- `vignettes/i_get_built.Rmd`, has `vignettes:` in yaml header
- `vignettes/i_do_not_get_built.Rmd`, does not have `vignettes:` in yaml header
- `.Rbuildignore`, which contains references to both vignette files

When I run `devtools::build()` then inspect the `tar.gz` file, I see `i_get_built.Rmd` and `i_get_built.html` in its `inst/doc` directory.

## Installation

You can install vignettebuild from github with:

```R
# install.packages("devtools")
devtools::install_github("vignettebuild/ijlyttle")
```



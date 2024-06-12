
<!-- README.md is generated from README.Rmd. Please edit that file -->

# jeeves

<!-- badges: start -->

[![Lifecycle:
experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/stages.html#experimental)
[![CRAN
status](https://www.r-pkg.org/badges/version/jeeves)](https://CRAN.R-project.org/package=jeeves)
[![R-CMD-check](https://github.com/venpopov/jeeves/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/venpopov/jeeves/actions/workflows/R-CMD-check.yaml)
<!-- badges: end -->

Jeeves assists in creating, managing and sharing reproducible research
projects in R. It provides tools for creating standard project
structures, managing dependencies, and generating reports with ease.

## Installation

You can install the development version of jeeves like so:

``` r
if (!requireNamespace("remotes", quietly = TRUE)) {
  install.packages("remotes")
} 
remotes::install_github("venpopov/jeeves")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(jeeves)
## basic example code
```

## Comparison with other packages

`jeeves` builds heavily on `usethis` to create research projects.
Whereas `usethis` is modular and general-purpose, `jeeves` provides
one-line functions for a complete project setup. After running one of
the main `jeeves` functions, you will be immediately ready to start
working on the code rather than setting up the project. By default,
`jeeves` sets up a project with:

- standard project directory structure
- package skeleton with filled out `DESCRIPTION`, `NAMESPACE`, `R/`,
  `tests/`, `LICENSE`, `README.Rmd`, `NEWS.md`, `.Rbuildignore`,
  `.gitignore files`
- version control via `git` and `GitHub`. A new repository is created on
  your GitHub account and the local project is linked to it
- package dependencies management via `renv` and installation of default
  development packages
- a pkgdown or a Quarto website for the package or the project. The
  website is automatically deployed to GitHub pages with a GitHub action
- continuous integration via GitHub actions for testing and deployment
- a skeleton `targets` pipeline for reproducible data analysis

Jeeves sets opinionated defaults for each of these steps, but you can
customize them by passing arguments to the main functions.

`usethis` is a fantastic package due to its modularity and flexibility.
At the same time, if you are like me, you might find yourself running
the same set of 20-30+ `usethis`, `git` and other functions every time
you start a new project. `jeeves` is an attempt to automate this process
and provide a one-stop-shop for setting up a new reproducible project.

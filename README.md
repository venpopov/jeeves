
<!-- README.md is generated from README.Rmd. Please edit that file -->

# jeeves

<!-- badges: start -->

[![Lifecycle:
experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/stages.html#experimental)
[![CRAN
status](https://www.r-pkg.org/badges/version/jeeves)](https://CRAN.R-project.org/package=jeeves)
[![R-CMD-check](https://github.com/venpopov/jeeves/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/venpopov/jeeves/actions/workflows/R-CMD-check.yaml)
<!-- badges: end -->

The goal of jeeves is to assist in creating, managing and sharing
reproducible research projects in R. It provides tools for creating
standard project structures, managing dependencies, and generating
reports with ease.

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

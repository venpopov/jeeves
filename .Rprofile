Sys.setenv(
  RENV_CONFIG_RSPM_ENABLED = FALSE,
  RENV_CONFIG_SANDBOX_ENABLED = FALSE
)

if (requireNamespace("rprofile", quietly = TRUE)) {
  rprofile::load(dev = quote(reload()))
} else {
  source("renv/activate.R")
}

reload <- function() {
  if (interactive() && requireNamespace("devtools", quietly = TRUE)) {
    devtools::document()
    devtools::load_all(quiet = TRUE)
  }
}

if (interactive()) {
  .quiet <- function(expr) {
    suppressMessages(suppressWarnings(expr))
  }

  .quiet(require(devtools))
  .quiet(require(reprex))
  .quiet(require(usethis))
  .quiet(require(gert))
  .quiet(require(targets))

  rm(.quiet)
}

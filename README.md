
<!-- README.md is generated from README.Rmd. Please edit that file -->

<!-- badges: start -->

[![CRAN
status](https://www.r-pkg.org/badges/version/prevederer)](https://cran.r-project.org/package=prevederer)
[![Travis build
status](https://travis-ci.org/wkdavis/prevederer.svg?branch=master)](https://travis-ci.org/wkdavis/prevederer)
[![AppVeyor build
status](https://ci.appveyor.com/api/projects/status/github/wkdavis/prevederer?branch=master&svg=true)](https://ci.appveyor.com/project/wkdavis/prevederer)
[![Codecov test
coverage](https://codecov.io/gh/wkdavis/prevederer/branch/master/graph/badge.svg)](https://codecov.io/gh/wkdavis/prevederer?branch=master)
<!-- badges: end -->

# prevederer

R package for accessing the Prevedere API. Access to the Prevedere API
requires an API key.

# Installation

``` r
devtools::install_github("wkdavis/prevederer") 
```

# Use

## Endpoints

  - `indicator`: returns basic information about an indicator.
  - `indicator_series`: returns the data for an indicator.
  - `correlation`: calculates Pearson’s r and other statistics at
    different offsets between an endogenous and exogenous indicator.
  - `raw_model`: returns all information about a forecast model.
  - `forecast`: returns historical fit and forecasted values of a
    forecast model.
  - `workbench`: returns the indicators used in a workbench.

## Example

``` r
library(prevederer)

api_key = "xyz123"
provider = "provider_a"
provider_id = "a123"

prevedere_indicator_series(api_key, provider, provider_id)
```

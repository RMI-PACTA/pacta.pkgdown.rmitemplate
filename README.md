
# pacta.pkgdown.rmitemplate <a href="https://rmi.org"><img src="man/figures/logo.png" align="right" height="31" /></a>

<!-- badges: start -->
[![Lifecycle: stable](https://img.shields.io/badge/lifecycle-stable-brightgreen.svg)](https://lifecycle.r-lib.org/articles/stages.html#stable)
<!-- badges: end -->

pacta.pkgdown.rmitemplate provides a custom pkgdown template for RMI PACTA R packages. Please don't use it for your own package if it's not a PACTA package.

inspired by [tidytemplate](https://github.com/tidyverse/tidytemplate/) and [rotemplate](https://github.com/ropensci-org/rotemplate)

meant to follow the limited documentation of a [pkgdown template](https://pkgdown.r-lib.org/articles/customise.html#template-packages)


## Installation

You can install the development version of pacta.pkgdown.rmitemplate from [GitHub](https://github.com/) with:

``` r
# install.packages("pak")
pak::pak("rmi-pacta/pacta.pkgdown.rmitemplate")
```


## Usage

Set it as your site's theme in `_pkgdown.yaml`:

``` yml
template:
  package: pacta.pkgdown.rmitemplate
```

If you're building your site using a GitHub action or other similar tool, you'll also need to install r2diitemplate in the runner. If you're using the [r-lib pkgdown workflow](https://github.com/r-lib/actions/blob/v2-branch/examples/pkgdown.yaml), you can add the following line to your DESCRIPTION:

    Config/Needs/website: rmi-pacta/pacta.pkgdown.rmitemplate

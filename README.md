
<!-- README.md is generated from README.Rmd. Please edit that file -->

<!-- badges: start -->

[![Travis build
status](https://travis-ci.org/overdodactyl/mayotemplate.svg?branch=master)](https://travis-ci.org/overdodactyl/mayotemplate)
[![Lifecycle:
experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
<!-- badges: end -->

## Overview

mayotemplate provides a custom [pkgdown](https://pkgdown.r-lib.org)
template for packages developed at Mayo Clinic. Please don’t use it for
your own package.

Inspired by [tidytemplate](https://github.com/tidyverse/tidytemplate/).

## Using mayotemplate

Include the following in your `_pkgdown.yaml` file:

``` yaml
template:
  package: mayotemplate
```

`mayotemplate` follows the same setup as `tidytemplate`. For more
documentation, please see their README file.

### Deploying a site on Travis-CI to Github Pages

If you are automatically deploying your site with Travis, add the
following in your `.travis.yml` file:

``` yaml
 before_cache:
    - Rscript -e 'remotes::install_github("overdodactyl/mayotemplate")'
```

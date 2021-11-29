
<!-- README.md is generated from README.Rmd. Please edit that file -->

# nloptr <img src='man/figures/logo.png' align="right" height="139" />

<!-- badges: start -->

[![R-CMD-check](https://github.com/astamm/nloptr/workflows/R-CMD-check/badge.svg)](https://github.com/astamm/nloptr/actions)
[![test-coverage](https://github.com/astamm/nloptr/workflows/test-coverage/badge.svg)](https://github.com/astamm/nloptr/actions)
[![Codecov test
coverage](https://codecov.io/gh/astamm/nloptr/branch/master/graph/badge.svg)](https://app.codecov.io/gh/astamm/nloptr?branch=master)
[![pkgdown](https://github.com/astamm/nloptr/workflows/pkgdown/badge.svg)](https://github.com/astamm/nloptr/actions)
[![CRAN
status](https://www.r-pkg.org/badges/version/nloptr)](https://CRAN.R-project.org/package=nloptr)
<!-- badges: end -->

**nloptr** is an R interface to
[NLopt](https://nlopt.readthedocs.io/en/latest/), a free/open-source
library for nonlinear optimization started by Steven G. Johnson,
providing a common interface for a number of different free optimization
routines available online as well as original implementations of various
other algorithms. It can be used to solve general nonlinear programming
problems with nonlinear constraints and lower and upper bounds for the
controls, such as

min<sub>*x* ∈ ℝ<sup>*n*</sup></sub>  *f*(*x*),

s.t. *g*(*x*) ≤ 0, *h*(*x*) = 0 and ℓ ≤ *x* ≤ *u*.

The [NLopt](https://nlopt.readthedocs.io/en/latest/) library is
available under the GNU Lesser General Public License (LGPL), and the
copyrights are owned by a variety of authors. See the
[website](https://nlopt.readthedocs.io/en/latest/Citing_NLopt/) for
information on how to cite NLopt and the algorithms you use.

## Installation

You can install **nloptr** from CRAN using:

    install.packages("nloptr")

Alternatively, you can install the development version from GitHub:

    # install.packages("remotes")
    remotes::install_github("astamm/nloptr")

The latest version 2.7.0 of the
[NLopt](https://nlopt.readthedocs.io/en/latest/) library will then be
automatically built using [CMake](https://cmake.org). The package will
try to find a [CMake](https://cmake.org) binary on your `PATH`. If it
cannot find one, the installation will fail with a message giving you
simple instructions for installing [CMake](https://cmake.org) first.
Alternatively, you can set an environment variable `CMAKE_BIN` pointing
to a [CMake](https://cmake.org) binary of your liking on your computer
for **nloptr** to use.

## Acknowledgments

I would like to express my sincere gratitude to [Dirk
Eddelbuettel](https://github.com/eddelbuettel), Uwe Ligges and [Jelmer
Ypma](https://github.com/jyypma) for the very instructive discussions
about the pros and cons of various build strategies in R packages.

## Reference

Steven G. Johnson, The NLopt nonlinear-optimization package,
<https://nlopt.readthedocs.io/en/latest/>

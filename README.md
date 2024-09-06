NeuroPartitioner
================

<!-- badges: start -->

[![USC
IMAGE](https://raw.githubusercontent.com/USCbiostats/badges/master/tommy-image-badge.svg)](https://image.usc.edu)
<!-- badges: end -->

## Installation Instructions

This document provides detailed steps to install the necessary
dependencies for the package. Please follow the instructions carefully
to ensure all dependencies are correctly installed.

### Step 1: Install devtools

The `devtools` package is essential for installing packages directly
from GitHub. If you do not have `devtools` installed, run the following
code:

``` r
if (!requireNamespace("devtools", quietly = TRUE))
    install.packages("devtools")
```

### Step 2: Install ANTsR

ANTsR is a critical package for medical image analysis in R. Install it
using devtools with the following command:

``` r
devtools::install_github('ANTsX/ANTsR')
```

### Step 3: Install fslr

The fslr package is an interface to the FSL (FMRIB Software Library)
tools. Install it from GitHub:

``` r
devtools::install_github("muschellij2/fslr")
```

### Step 4: Install EveTemplate

The EveTemplate package can be installed using remotes. First, ensure
that remotes is installed:

``` r
if (!requireNamespace("remotes", quietly = TRUE))
    install.packages("remotes")
```

Then install EveTemplate:

``` r
remotes::install_github("neuroconductor/EveTemplate")
```

### Step 5: Install extrantsr

extrantsr is another package essential for neuroimaging data analysis.
Install it using:

``` r
devtools::install_github("muschellij2/extrantsr")
```

### Step 6: Install FSL

FSL is not an R package but a standalone software suite for MRI and fMRI
analysis. Follow the instructions on \[their website\]
(<https://fsl.fmrib.ox.ac.uk/fsl/docs/#/install/index>) to download and
install it.


<!-- README.md is generated from README.Rmd. Please edit that file -->

# FindIT2

<!-- badges: start -->
<!-- badges: end -->

The goal of `FindIT2` is to …

## Installation instructions

`FindIT2` is available on Bioconductor, you can install it by:

``` r
if (!requireNamespace("BiocManager", quietly = TRUE)) {
    install.packages("BiocManager")
}

BiocManager::install("FindIT2")
```

> For the packages on bioconductor, please make sure you download the
> latest stable `R` release from [CRAN](http://cran.r-project.org/)

If you want the development version, install it directly from
[GitHub](https://github.com/shangguandong1996/FindIT2):

``` r
BiocManager::install("shangguandong1996/FindIT2")
```

## Document

If you want to download development version from github and view vignettes using
`browseVignettes(FindIT2)`, your R version should be 4.0 or greater
according to this
[issue](https://github.com/Bioconductor/BiocStyle/issues/78) because I
use the BiocStyle to output rmarkdown. Then you have to firstly download
the below packages

``` r
packages <- c("BiocStyle", "knitr", "rmarkdown", "sessioninfo", "TxDb.Athaliana.BioMart.plantsmart28")
installed_packages <- packages %in% rownames(installed.packages())
if (any(installed_packages == FALSE)) {
    BiocManager::install(packages[!installed_packages])
}
```

Meanwhile, adding the `build_vignettes=TRUE` when downloading
development version

``` r
BiocManager::install("shangguandong1996/FindIT2", build_vignettes=TRUE)
```

To view documentation of FindIT2, start R and enter:

``` r
browseVignettes("FindIT2")
```

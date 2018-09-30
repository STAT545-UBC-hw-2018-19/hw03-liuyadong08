STAT545 Homework 03 The use of dplyr/ggplot2
================

## Overview

This Rmarkdown file aims to explore the gapminder dataset with **dplyr**
package, and to plot figures using **ggplot2** package. It will be used
as a cheatsheet for future data manipulation and figure plotting.

## Import data frame and tidyverse pacakge

Gapminder data will be used in this homework, and the dataset will be
explored using “tidyverse” package.

``` r
library(gapminder)
library(dplyr)
```

    ## 
    ## Attaching package: 'dplyr'

    ## The following objects are masked from 'package:stats':
    ## 
    ##     filter, lag

    ## The following objects are masked from 'package:base':
    ## 
    ##     intersect, setdiff, setequal, union

``` r
# use suppressMessages(library(tidyverse)) to generate a pdf file
```

``` r
gapminder %>% 
  select(pop)
```

    ## # A tibble: 1,704 x 1
    ##         pop
    ##       <int>
    ##  1  8425333
    ##  2  9240934
    ##  3 10267083
    ##  4 11537966
    ##  5 13079460
    ##  6 14880372
    ##  7 12881816
    ##  8 13867957
    ##  9 16317921
    ## 10 22227415
    ## # ... with 1,694 more rows

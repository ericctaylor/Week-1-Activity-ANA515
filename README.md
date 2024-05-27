# Week-1-Activity-ANA515
> library(ggplot2)
> library(dplyr)

Attaching package: ‘dplyr’

The following objects are masked from ‘package:stats’:

    filter, lag

The following objects are masked from ‘package:base’:

    intersect, setdiff, setequal, union

> smaller <- diamonds %>% 
+   filter(carat <= 1)
> smaller %>% 
+   ggplot(aes(carat)) + 
+   geom_freqpoly(binwidth = 0.01)

---
title: "Regression-Example"
author: "Jason West"
date: "2024-03-09"
output:
  bookdown::html_document2:
    keep_md: yes
  html_document:
    df_print: paged
summary: How to run a basic regression
authors: admin
slug: "Regression-Example"
categories: Blogging
tags:
- Regression
- R
- Blogging
- Markdown
- R Markdown
subtitle: How to run a basic regression.
---



## R Markdown

This is an R Markdown document. Markdown is a simple formatting syntax for authoring HTML, PDF, and MS Word documents. For more details on using R Markdown see <http://rmarkdown.rstudio.com>.

When you click the **Knit** button a document will be generated that includes both content as well as the output of any embedded R code chunks within the document. You can embed an R code chunk like this:


```r
summary(cars)
```

```
##      speed           dist       
##  Min.   : 4.0   Min.   :  2.00  
##  1st Qu.:12.0   1st Qu.: 26.00  
##  Median :15.0   Median : 36.00  
##  Mean   :15.4   Mean   : 42.98  
##  3rd Qu.:19.0   3rd Qu.: 56.00  
##  Max.   :25.0   Max.   :120.00
```

## Including Plots

You can also embed plots, for example:

![](sample_files/figure-html/pressure-1.png)<!-- -->

Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.


```r
fit=lm(dist~speed,data=cars)
b=coef(fit)
plot(cars)
abline(fit)
```

![](sample_files/figure-html/unnamed-chunk-1-1.png)<!-- -->

The slope of the regression is -17.5790949.

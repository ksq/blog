---
title: How to merge two columns of two tables in R
author: ~
date: '2020-04-19'
slug: how-to-merge-two-columns-of-two-tables-in-r
categories: []
tags: []
---

When we need to merge two columns from two different data sets, we could use `merge` function. 
For example, 

```r
rdt3 <- merge(rdt1[, .(symbol, year, x1), 
    rdt2[, .(symbol, year, x2)], 
    by = c("symbol", "year"), all.x = TRUE])
```

We get the dataset of rdt3 which includes four columns `symbol`, `year`, `x1`, `x2`.


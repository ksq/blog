---
title: How to view the values of two columns in one table in R
author: ~
date: '2020-04-26'
slug: how-to-view-the-values-of-two-columns-in-one-table-in-r
categories: []
tags: []
---

When we would like to view the values of some columns in one dataset, we could input the name of the dataset, select the "key" columns and the target columns. 
For instance, 

```r
rdt[, .(symbol, year, x1, x2)]
```
We could view a dataset with four columns `symbol`, `year`, `x1`, `x2`.
The columns of `symbol`, `year` are the "key" columns for identification while the columns of `x1` and ``x2` are the ones that we would like to view.
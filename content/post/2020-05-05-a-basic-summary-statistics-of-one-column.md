---
title: A basic summary statistics of one column
author: ~
date: '2020-05-05'
slug: a-basic-summary-statistics-of-one-column
categories: []
tags: []
---

When we would like to view the basic summary statistics of one column, we could use the "summary" function. 
For example, 

```r
rdt[, summary(x)]
```

We could see the minimum, 1st quater, median, mean, 3rd quater and maximum value of this column.
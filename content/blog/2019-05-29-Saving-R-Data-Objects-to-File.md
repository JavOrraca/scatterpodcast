+++
authors = ["Javier Orraca",]
title = "Saving R Data Objects"
date = "2019-05-29"
tags = ["blog",]
images = ["R-Data-Formats.jpg",]
+++

Are you spending too much time reading large data sets, wrangling, then waiting to convert your data frames to matrices or arrays?
<!--more-->
If you're like me, you might be doing a lot of this locally... And then all of the sudden, you've got 25-50 GB (or more) worth of vector objects sitting in your environment and it's taken 10-15 minutes to even get to this point where you can begin modeling...

Here's a solution for you: Use R to save one or multiple data objects to file as RDS or RData files. I got this amazing tip from [Emil Hvitfeldt](https://www.hvitfeldt.me/blog/) and I've already saved significant time from this recommendation.

Source:

* [STHDA Guide for Saving RDS and RData files](http://www.sthda.com/english/wiki/saving-data-into-r-data-format-rds-and-rdata)
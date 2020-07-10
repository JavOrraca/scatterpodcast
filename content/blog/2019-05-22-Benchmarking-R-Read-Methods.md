+++
authors = ["Javier Orraca",]
title = "Benchmarking CSV File Read Times"
date = "2019-05-22"
tags = ["blog",]
images = ["BenchmarkingR.jpg",]
+++

I have been running code for a client project and each CSV file is 300MB with over 400,000 records. Base R was not cutting it for me and I was wasting too much time staring at my local system waiting for my files to be read. So...
<!--more-->
I found the microbenchmark package and started exploring faster file read methods relative to base R. I discovered Tidyverse's readr and vroom packages, and while I had used the data.table package many times, I did not realize that data.table had its own file read function (i.e., "fread"). To evaluate the different read methods, I loaded my csv data set 10 times using each method and plotted the results above. At least for my purely numerical data set, data.table was the clear winner followed by vroom. One major caveat here is that not all of these methods are made equal... Per the Tidyverse vroom writeup:
* "The main reason *vroom* can be faster is because character data is read from the file lazily; you only pay for the data you use. This lazy access is done automatically, so no changes to your R data-manipulation code are needed."
* I believe data.table operates in a similar pay-as-you-play manner

The above visualization was done in R using the microbenchmark package, ggplot2 for base plotting framework, and ggthemes package for _The Economist_ color theme and styling.

File Read Sources:

* [Tidyverse's readr](https://readr.tidyverse.org/)
* [data.table on GitHub](https://github.com/Rdatatable/data.table/wiki)
* [Tidyverse's vroom](https://www.tidyverse.org/articles/2019/05/vroom-1-0-0/)

Visualization Sources:

* [microbenchmark](https://cran.r-project.org/web/packages/microbenchmark/index.html)
* [ggplot2](https://ggplot2.tidyverse.org/)
* [ggthemes](https://www.ggplot2-exts.org/ggthemes.html)
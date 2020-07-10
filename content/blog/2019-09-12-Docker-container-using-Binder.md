+++
authors = ["Javier Orraca",]
title = "Docker containers using Binder"
date = "2019-09-12"
tags = ["blog",]
images = ["binder.jpg",]
+++

I've spent weeks slowly learning how to build and deploy Docker containers... It is dense for beginners but I was elated to find an easier approach to building a Docker image with all the necessary packages and dependencies that you need, and deploying an interactive web notebook using RStudio or Jupyter notebooks.
<!--more-->
Some setup is involved, granted, the process is significantly streamlined with Binder. There is one main caveat here - Your data must be on a GitHub repo. Thank you Tony Hirst for writing about this on R-bloggers! Check out the links below for the R-bloogers post and introduction to Binder (for R users), including a few working Binder examples:

Links to learn more about Binder:

* R-bloggers: [Running R Projects in MyBinder, by Tony Hirst](https://www.r-bloggers.com/running-r-projects-in-mybinder-dockerfile-creation-with-holepunch/)
* Deployable Binder example: [Using R with RStudio](https://mybinder.org/v2/gh/binder-examples/r/master?urlpath=rstudio)
* Deployable Binder example: [Using Python + R on JupyterLab](https://mybinder.org/v2/gh/binder-examples/r_with_python/master?urlpath=lab)
* Binder's GitHub: [More environment examples](https://github.com/binder-examples)
* Binder's homepage: [https://mybinder.org/](https://mybinder.org/)
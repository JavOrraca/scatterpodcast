+++
authors = ["Javier Orraca",]
title = "TensorFlow 2.0 for R"
date = "2019-10-07"
tags = ["blog",]
images = ["TensorFlow2.jpg",]
+++

TensorFlow 2.0 is finally alpha-released. I use Python and R but tend to focus on R these days. So, what changes should R users be aware of? The RStudio team wrote a great overview on the subject.
<!--more-->
The RStudio team wrote a great overview of the new `r-tensorflow` ecosystem, with code samples. The good news? If you've been using TensorFlow within `keras`, like me, syntactically almost everything remains the same. You'll notice very few differences, if any. For those unfamiliar with `keras`, it is the frontend library for machine learning and AI that uses TensorFlow for AI and deep learning as a low-level backend. Two updates that I'm excited to explore include 1) `tfdatasets` for data pipelining, and 2) TensorFlow Hub (available as the R `tfhub` package) for publishing and using pre-trained models.

Links:

* RStudio Blog: [TensorFlow 2.0 is here - what changes for R users?](https://blogs.rstudio.com/tensorflow/posts/2019-10-08-tf2-whatchanges/)
* TensorFlow Hub: [Existing Pretrained Models](https://tfhub.dev)
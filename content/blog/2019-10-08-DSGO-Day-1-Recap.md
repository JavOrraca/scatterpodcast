+++
authors = ["Javier Orraca",]
title = "DataScienceGO Day 1"
date = "2019-10-08"
tags = ["blog",]
images = ["sanjeev.jpg",]
+++

DataScienceGO (DSGO) was a huge success for my second visit. It was great to reconnect with data science practitioners and leaders that I met at DSGO in 2018, and to learn about the latest trends. A lot has changed in the space in just one year.
<!--more-->
I felt a lot of pride seeing UCI's MS in Business Analytics ("MSBA") program as the main educational sponsor for the event, and I also enjoyed seeing my old professor, [Sanjeev Dewan](https://www.linkedin.com/in/sanjeev-dewan-75302b17/), talk on the main stage about causal inference methods in data science (that's him in the picture, above)!

The takeaways and resources below were some of my favorite from Day 1, and I plan to follow up with a second post covering DSGO Day 2 highlights. Shoot me a note if you have any questions and I hope these help you!

Download the DSGO 2019 presentations (PDF format):

* [DSGO 2019 Presentations](https://drive.google.com/open?id=1rRbkp_LY2NC9UCi7iIR7BdDAKKcolVVe)

Day 1 Takeaways and Resources (by presenter):

* [Sarah Aerni](https://www.linkedin.com/in/sarahaerni/), Director of Data Science at Salesforce
   * Embrace data science experimentation, especially on deployed models. For example, if a model is performing poorly one month, do a deep dive to understand the drivers for _why_ that model is performing poorly.
   * [TransmogrifAI](https://transmogrif.ai) - This is Salesforce's open-source, AutoML library for structured data, written in Scala and running on top of Apache Spark.
   * Use a test-driven development approach to data science, e.g., using synthetic data for scenario testing and model performance evaluation.
* [Gabriela de Queiroz](https://www.linkedin.com/in/gabrieladequeiroz/), Founder of R-Ladies and Data Science Manager at IBM
   * At IBM, Gabriela works for the [Center for Open-Source Data and AI Technologies ("CODAIT")](https://developer.ibm.com/code/open/centers/codait/about/). Their mission is to make "AI technologies accessible to the practitioners that understand real-world problems, so that they themselves can develop AI solutions that solve these problems."
   * CODAIT's [catalog of open-source projects](https://developer.ibm.com/code/open/centers/codait/projects/) is impressive... At the conference, we saw a demo of CODAIT's [Model Asset eXchange](https://developer.ibm.com/exchanges/models/), a place for free, deployable, and trainable deep learning models.
   * Some of the most accomplished data scientists that I know, I met through R-Ladies of Irvine. I was super impressed to find out that Gabriela is the founder of the [R-Ladies Global](https://rladies.org) organization.
* [Sanjeev Dewan](https://www.linkedin.com/in/sanjeev-dewan-75302b17/), Professor of Information Systems and Director of UCI's MSBA Program
   * Professor Dewan discussed a topic that I don't see practitioners discussing nearly enough, i.e., causal inferences can be made using randomized experiments and non-experimental methods. The two examples he covered included Diff-in-Diff and Propensity Score Matching.
   * Difference-in-Differences Estimation example: _Minimum Wages and Employment: A Case Study of the Fast-Food Industry in New Jersey and Pennsylvania_, by David Card and Alan Krueger
      * Link to Diff-in-Diff study: [Berkeley's research library](http://davidcard.berkeley.edu/papers/njmin-aer.pdf)
   * Propensity Score Matching ("PSM") using R: [R Tutorial on GitHub, with code](https://sejdemyr.github.io/r-tutorials/statistics/tutorial8.html)
* [Pawel Skrzypek](https://www.linkedin.com/in/pawel-skrzypek-836344/), CTO at AI Investments Ltd.
   * Some of my favorite machine learning problems are time-series financial forecasting problems, and Pawel really impressed the crowd here.
   * He covered stacked LSTM and CNN models (ensemble models or "super learners") for forecasting and portfolio optimization with AI.
   * He educated me on the [M4 Competition](https://www.mcompetitions.unic.ac.cy), one of the most important annual forecasting events on the planet. This is a super interesting competition that I plan to follow in the years to come.
   * Not explicitly covered in Pawel's presentation, but something that I found interesting... In 2018, one of Uber's leading data scientists, Slawek Smyl, was named the winner of the 2018 competition. He built a hybrid-model including exponential smoothing ("ES") and a black-box recurrent neural network ("RNN") forecasting engine that he coded in C++ and DyNet, using R and SQL to manipulate and merge the output data. Link: [M4 Forecasting Competition: Introducing a New Hybrid ES-RNN Model](https://eng.uber.com/m4-forecasting-competition/)
* [Hadelin de Ponteves](https://www.linkedin.com/in/hadelin-de-ponteves-1425ba5b/), Co-Founder & Director at BlueLife AI
   * Hadelin covered traditional natural language processing ("NLP") approaches and provided the audience with a demo of the newest NLP method using Transformers (faster, more accurate, less training involved).
   * Examples: Google's BERT, Facebook's RoBERTa, XLM, XLNet
   * Learning resource: [Transformers on Hugging Face](https://huggingface.co/transformers/)
   * Note: As of the date of this article, Google recently released a leaner version of BERT called "ALBERT" that uses advanced feature reduction and is topping the NLP leaderboards. Source: [VentureBeat.com](https://venturebeat.com/2019/09/26/google-ais-albert-claims-top-spot-in-multiple-nlp-performance-benchmarks/)
* [Ben Taylor](https://www.linkedin.com/in/bentaylordata/), Co-Founder and Chief AI Officer of Zeff.ai
   * I recently interviewed Ben for [episode 21 of Scatter Podcast](https://www.javierorraca.com/scatterpodcast/episode-021/), so this was a treat to see live his first public demo of his AI-powered, Xbox Live _Call of Duty_ player enhancement tool (something that Xbox and Microsoft are unable to detect).
   * For this project, he trained his AI models using video, audio, and controller signals recorded from one of the top _Call of Duty_ players in the world. His ensemble model had roughly 30-models concurrently running, with low latency, and trained using an Intel beast of a server with 196-cores and 12TB of RAM.
   * While online games are fun, Ben paints a sinister picture of what world governments could be doing, i.e., recording and training AI agents based on kill sequences from online games, improving themselves while developing AI technologies that could outperform humans if deployed for use in war... Scary!
   
Unfortunately, I did not make it to Day 2 but I will try to collect similar notes from friends that attended DSGO Day 2.
+++
authors = ["Javier Orraca",]
title = "Salesforce Stock Price Prediction"
date = "2019-06-13"
tags = ["blog",]
images = ["Salesforce.jpg",]
+++

Where will Salesforce stock be at the end of 2019? I'm predicting $178.40. I used R to produce a multi-variate time series model and Tableau to visualize historical CRM stock prices (the grey line) vs my model (the blue line), including my Dec 2019 prediction (red dot).
<!--more-->
The model was built in February using historical stock price data from 2004 to 2018. Play around with the Tableau viz (link below)!

Independent Variables:

* U.S. consumer sentiment index (published by the University of Michigan)
* GDP
* CRM historical stock prices
* Other tech stocks (IBM, Oracle, SAP)
* Month (as categorical, for seasonality)

High-level model process:

* Linear regression model created for log-transformed historical data
* Uni-variate ARIMA time series models produced for each independent variable (excluding month)
* ARIMA model output used to predict monthly 2019 data points and these data points were then log-transformed
* Log-transformed ARIMA data points joined into one data set and processed as input to the original linear regression model created above
* Linear regression score outputs were exponentiated
* The model coefficients were incorporated into Tableau for a "what-if" style interactive visualization

Source:

* [Javier's Salesforce Stock Prediction on Tableau Public](https://public.tableau.com/profile/javier.orraca#!/vizhome/SalesforceStockPrediction/StockPrediction)
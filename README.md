# Adidas-Time-Series-Forecasting
To forecast Adidas future revenues from Q2 of 2017 to Q4 of 2018, applying Time Series Theories to predict whether the goal of ADIDAS can be reached.
ADIDAS AG is a multinational corporation, founded and head-quartered in Herzogenaurach, Germany,that designs and manufactures shoes, clothing and accessories. It is the largest sportswear manufacturer in Europe, and the second largest in the world, after Nike. 
In the fiscal year of 2016, ADIDAS generated a total revenue of $19,068 million, increased by 18 percent. In its annual report, ADIDAS projects an annual growth in sale between 11 percent and 13 percent


***Featured technologies***
R Studio: RStudio is dedicated to sustainable investment in free and open-source software for data science.
fpp - the fpp package, available on CRAN, using library(fpp). This will automatically load several other packages including forecast and ggplot2, as well as all the data used in the book Forecasting: principles and practice'' by Rob JHyndman and George Athanasopoulos.
knitr - The R package knitr is a general-purpose literate programming engine, with lightweight API's designed to give users full control of the output without heavy coding work 
forecastHybrid - The "forecastHybrid" package provides functions to build composite models using multiple individual component models from the "forecast" package. These hybridModel objects can then be manipulated with many of the familiar functions from the "forecast" and "stats" packages including forecast(), plot(), accuracy(), residuals(), and fitted()
TSA - Contains R functions and datasets detailed in the book "Time Series Analysis with Applications in R (second edition)" by J.D. Cryer and K.S. Chan
CADFtest - A Package to Perform Covariate Augmented Dickey-Fuller Unit Root Tests

***BOX JENKIN MODEL***


**Exploratory Data Analysis**: Here, we plot the time series plot, auto-correlation function(ACF) plot, partial auto-correlation function(PACF) plot, and EACF of the time series. 

**Finding Models**: Here, we find the models by checking the number of bars in ACF plot to find the MA(q) and number of bars in PACF to find the AR(p) and then cross check it with EACF to find ARMA(p,q) model.

**Stationarity**: Here, we test for stationarity of the TS by Augmented Dicky Fuller test. If the TS is stationary we proceed to the next step, otherwise if the TS is non-stationary, we apply differencing,transforming, and detrending to remove stationarity from the TS and then use Augmented Dicky Fuller test to test for stationarity again.

**Parameter Estimation** : we compare multiple models based on the AIC and BIC scores, log likelihood values, Adjusted Pearson Goodness-of-Fit Test, Ljung-Box Test, ARCH LM Tests etc and select the best model from them.

**Residual Analysis** : Here, we analyse the residuals of the bets model by making ACF plot, Histogram, QQ plot, Residual plot and check for Shapiro-Wilk test and Ljung-Box test.

**Prediction**: Here, we use the best model to forecast the revenue of Adidas

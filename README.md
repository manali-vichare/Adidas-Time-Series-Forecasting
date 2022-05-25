# Adidas-Time-Series-Forecasting
To forecast Adidas future revenues from Q2 of 2017 to Q4 of 2018, applying Time Series Theories to predict whether the goal of ADIDAS can be reached.
ADIDAS AG is a multinational corporation, founded and head-quartered in Herzogenaurach, Germany,that designs and manufactures shoes, clothing and accessories. It is the largest sportswear manufacturer in Europe, and the second largest in the world, after Nike. 
In the fiscal year of 2016, ADIDAS generated a total revenue of $19,068 million, increased by 18 percent. In its annual report, ADIDAS projects an annual growth in sale between 11 percent and 13 percent




***BOX JENKIN MODEL***


**Exploratory Data Analysis**: Here, we plot the time series plot, auto-correlation function(ACF) plot, partial auto-correlation function(PACF) plot, and EACF of the time series. 

**Finding Models**: Here, we find the models by checking the number of bars in ACF plot to find the MA(q) and number of bars in PACF to find the AR(p) and then cross check it with EACF to find ARMA(p,q) model.

**Stationarity**: Here, we test for stationarity of the TS by Augmented Dicky Fuller test. If the TS is stationary we proceed to the next step, otherwise if the TS is non-stationary, we apply differencing,transforming, and detrending to remove stationarity from the TS and then use Augmented Dicky Fuller test to test for stationarity again.

**Parameter Estimation** : we compare multiple models based on the AIC and BIC scores, log likelihood values, Adjusted Pearson Goodness-of-Fit Test, Ljung-Box Test, ARCH LM Tests etc and select the best model from them.

**Residual Analysis** : Here, we analyse the residuals of the bets model by making ACF plot, Histogram, QQ plot, Residual plot and check for Shapiro-Wilk test and Ljung-Box test.

**Prediction**: Here, we use the best model to forecast the revenue of Adidas

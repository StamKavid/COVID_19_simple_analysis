# COVID-19 Forecasting: Project Overview

In this project you will find Covid-19 cases prediction for the next 30 days, using Facebook Prophet model. More specifically:
* Visualization of daily COVID-19 cases (Globally & **Greece**)
* Visualization of daily COVID-19 death cases (Globally & **Greece**)
* Geographical visualization (Globally)
* COVID-19 Cases prediction for next 30 days (Globally & **Greece**)

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Resources used

**Python Version:** 3.7

**Fbprophet Version:** 0.6

**Pystan Version:** 2.19

**Packages:** numpy, pandas, matplotlib, plotly, sklearn

**Fbprophet article:** https://medium.com/tokopedia-data/hacking-time-series-forecasting-like-a-pro-with-fbprophet-76f276f0a058#:~:text=What%20is%20FBProphet%3F,x)%20%2B%20e(t)


# Time-Series Forecasting

The purpose of time series analysis is generally twofold: to understand or model the stochastic mechanisms that gives rise to an observed series and to predict or forecast the future values of a series based on the history of that series

Time-series forecast itself is one of the methods to create a model for predicting future values based on current and historical time series data. There are four components of time-series:

1. **Trend**: an increase or decrease of data; could be linear or nonlinear (logistics growth)
2. **Seasonality**: a characteristic of time-series data when it experiences regular and predictable movement after a fixed period of time
3. **Cyclic**: a cyclic pattern exists when the data experience rises or falls (regular or periodic fluctuation in data)
4. **Irregularity**: the residual of time series after the trend-cycle and seasonal component are removed

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Facebook Prophet

It’s a tool intended to help you to do time series forecasting at a scale with ease. It uses decomposable time series model with 3 main components: **seasonal**, **trends**, **holidays** or **events** effect and error which are combined into this equation:

***f(x) = g(x) + s(x) + h(x) + e(t)***

where,

g(x) is a trend function which models the non-periodic changes. It can be either a linear function or a logistic function.
s(x) represents a periodic changes i.e weekly, monthly, yearly. A yearly seasonal component is modeled using Fourier series and weekly seasonal component using dummy variables.
h(x) is a function that represents the effect of holidays which occur on irregular schedules.(n ≥ 1 days)
e(x) represents error changes that are not accommodated by the model.

Here you can find the paper for Facebook prophet: https://peerj.com/preprints/3190.pdf#section.1
Here you can find the GIT page of FBProphet: https://github.com/facebook/prophet

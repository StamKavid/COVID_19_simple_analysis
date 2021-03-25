# COVID_19_simple_analysis
In this project you will find Covid-19 cases prediction for the next 30 days, using Facebook Prophet model.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

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

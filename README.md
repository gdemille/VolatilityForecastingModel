# VolatilityForecastingModel
Use this code to automatically pull in financial data from yahoo finance, transform the data into a usable database, then perform a SARIMAX and GARCH analysis to forecast volatility for the given inputs.
In it's current form, the SARIMAX model uses SPY returns as the endogenous variable and the VIX as an exogenous variable. The residuals from the SARIMAX model are subsequently used as the inputs for the GARCH model, which is then used to forecast volatility for SPY.

Next update: how to include ACF & PACF tests to ensure data stationarity, and how to perform a Ljung-Box test on the residuals to test for autocorrelation of the residuals.

# Oracle-Price-Analysis
This analysis examines Oracle's stock price behavior, including data preprocessing, descriptive statistics, visualizations, time series, and predictive modeling. Key findings show a significant upward price trend and a positive correlation between trading volume and prices, offering insights for informed investor decisions based on historical data.

**Introduction**

Oracle's stock prices are used for a variety of purposes by different stakeholders. Investors use stock prices to decide when to buy or sell Oracle shares based on their investment strategies. Stock prices help in managing and rebalancing investment portfolios to maintain desired asset allocations. . Understanding stock price movements allows stakeholders to make informed decisions, manage risks, and capitalize on market opportunities. The objective of the study is understanding Oracle's stock price behavior over time, highlighting trends, volatility, and conducting potential predictive modeling approaches on stock prices. The significance of this study is it provides a comprehensive understanding of Oracle's stock price behavior over time, highlighting trends, volatility, and potential predictive modeling approaches. The insights can aid investors and analysts in making informed decisions based on historical data and forecasts.

**Theory and Methodology**

Data Acquisition: The dataset was downloaded from Kaggle and loaded into a Jupyter notebook.

Data Preprocessing: Missing values were identified and necessary adjustments made.

Descriptive Statistics: Summary statistics were generated using Python.

Price Visualization: Closing price variations over time were plotted to understand stock behavior.

Volume Visualization: Trading volume changes were visualized, revealing patterns linked to events and price movements.

Time Series Decomposition: The 'close' variable was decomposed to identify trends and seasonality, enhancing forecasting accuracy.

Rolling Statistics: Rolling mean and standard deviation were calculated to assess trends and volatility in closing prices.

Stationarity Testing: The ADF test was performed to check if the closing price data is stationary.

ACF and PACF Plots: Autocorrelation functions were analyzed to inform ARIMA modeling parameters.

ARIMA Modeling: The ARIMA model was applied for forecasting closing stock prices, addressing time series characteristics.

GARCH Modeling: As ARIMA was unsuitable, the GARCH model was used for volatility forecasting, capturing time-varying volatility.

Daily Returns Plot: Daily returns were plotted to assess volatility and market behavior.

Price vs. Volume Regression: A regression plot was created to explore the relationship between stock price movements and trading volume, aiding in strategy development.

This methodology provides a structured approach to analyzing Oracle's stock prices, offering insights for informed investment decisions.

**Exploratory Data Analysis**

**The plot of oracle socks closing prices over time.**

![image](https://github.com/user-attachments/assets/dc777fb4-f947-4b35-9d49-a833729b7f31)



**Oracle stock trading volume over time.**

![image](https://github.com/user-attachments/assets/868230c2-7f73-465d-8750-9c75dec19399)

**Time series decomposition**


![image](https://github.com/user-attachments/assets/35257e67-c45e-41e8-a162-c30911e7b048)


**Advanced analysis**

![image](https://github.com/user-attachments/assets/2e0684f3-0d19-4b3e-a7b3-9be053c0196e)


The rolling mean is same as the close price and the there is no large variation in the standard deviation with time.

![image](https://github.com/user-attachments/assets/90ef610a-a75e-4557-b17b-f8051f651c39)

![image](https://github.com/user-attachments/assets/6960867c-051f-422a-8e9c-25940f139127)

![image](https://github.com/user-attachments/assets/2a736b79-7d25-489f-9b1d-d7c751ab4e16)


ARIMA is not giving a valuable output. So ARIMA is not suitable to capture volatility dynamics.


![image](https://github.com/user-attachments/assets/c3c752c4-9dc5-43cf-b1d9-49be7e31c367)

The output from fitting a GARCH model to Oracle's stock price data indicates that the model was successfully optimized to provide a good fit, as reflected by the significantly improved negative log-likelihood value. This suggests that the GARCH model is suitable for capturing the volatility dynamics observed in Oracle's stock returns, making it useful for risk management, forecasting volatility, and other financial analyses.


![image](https://github.com/user-attachments/assets/5701073d-9bc5-459a-8f7b-8035398f8f02)

The plot suggests that Oracle's stock experienced major volatility in the past which may have been impacted by specific events such as dot-com bubble or financial crisis.


![image](https://github.com/user-attachments/assets/593e7d44-6a6c-4537-8d9d-5bbbdf8d18e0)

There is a negative correlation between the stock price and the trading volume of oracle.


**Conclusion**

• The stock's closing price shows an upward trend over time.

• Trading volume exhibits high volatility, with significant spikes at certain periods.

• GARCH model is more suitable than ARIMA model to model this data.

• Daily returns exhibit significant volatility, characteristic of stock market behavior.

• There is a negative relationship between trading volume and stock prices.



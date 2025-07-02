# Indian-Railway-Sector-Stocks

Analyzing Co-Movement and Lead-Lag Effects in Indian Railway Sector Stocks


**PROJECT OBJECTIVE**
The goal is to statistically validate the observed synchronized movement of Indian railway stocks, identify any lead-lag relationships (where one stock's price movement consistently precedes another's), and potentially build a basic predictive model.

**DATA COLLECTION AND PREPRARTION**
Stocks to Analyze: Start with a list of prominent railway-related stocks. Key players in this sector include:
  > Indian Railway Finance Corp Ltd. (IRFC)
  > IRCTC Ltd.
  > Rail Vikas Nigam Ltd. (RVNL)
  > Ircon International Ltd.
  > RITES Ltd.

 Data Sourcing: Uses Python library "yfinance" to download historical daily stock price data (Open, High, Low, Close, Volume) for these companies.

 Data Cleaning: (Though in my cases it was needed but still) -- I uses Forward Fill (ffill) Method. It is used to fill misssing NaN values it propagates the last known value forward to the next missing values.

 ----------------Exploratory Data Analysis (EDA)----------------
 1. Visual Confirmation
 2. Correlation Analysis

----------------Statistical Analysis----------------
1. Stationarity Testing
2. Cointegration Analysis
3. Lead-Lag Effect Identification    ----- Granger Causality Test: This statistical hypothesis test helps determine if one time series is useful for forecasting another. AND Cross-Correlation: Calculate the cross-correlation function (CCF) between pairs of stock returns to see if one series leads the other.


TOOLS:-
+++++  LANGUAGE: Python
+++++  LIBRARIES: |Pandas: For data manipulation and analysis.|__|NumPy: For numerical operations.|__|Statsmodels: For conducting statistical tests (ADF, Johansen, Granger causality) and fitting time series models like VAR.|__|yfinance: For downloading stock market data.| 

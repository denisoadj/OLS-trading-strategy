# OLS-trading-strategy

This repository applies linear OLS regression to predict the direction of market movements based on historical log returns. 

To keep things simple, only two features are used. The first feature (lag_1) represents the log returns of the financial time series lagged by one day. The second feature (lag_2) lags the log returns by two days. Log returns in contrast to prices are stationary in general, which often is a necessary condition for the application of statistical and ML algorithms. 

The basic idea behind the usage of lagged log returns as features is that they might be informative in predicting future returns. For example, one might hypothesize that after two downward movements an upward movement is more likely (“mean reversion”), or, to the contrary, that another downward movement is more likely (“momentum” or “trend”). The application of regression techniques allows the formalization of such informal reasonings.

In this article, I present a code I wrote in Python that is used to analyze Bitcoin prices. The method used is a machine learning based approach with AdaBoost Regression. This code offers great potential for those who want to perform financial analysis, create price predictions and develop trading strategies.
First of all, I imported the libraries I will use in the code.
In the first step, I pulled Bitcoin price data with the symbol "BTC-USD" using the yfinance library. You can also pull the price of any index or stock. I also limited this data to the date "2023-01-01" as I wanted to analyze this data over a more recent time period.
I then added a date column to this data to be able to do date-related operations. This is important for time series analysis.
I chose independent and dependent variables to process the data. The independent variable is set to "Date_Int" as a representation of the date column, while Bitcoin prices ("Close") are chosen as the dependent variable.
In this step, I created an AdaBoostRegressor model. AdaBoost is used to boost a regression model using decision trees. The model limits the depth of the trees.
The model is trained on the selected dataset. This training aims to predict future prices using historical price data.
Using the trained model, I obtained forecasts of future Bitcoin prices. I visualized these forecasts and the actual price data on a graph on a logarithmic scale. The reason for using logarithmic instead of linear graphs is that it is much more convenient and readable, especially over large time periods. This visualization shows how forecasts can be compared to actual data.
In particular, this code can help developers of financial software to create applications that predict the future prices of various stocks and indices. In addition, various financial reports can be generated by outputting the values of the code.

![image](https://github.com/YavuzAkbay/AdaBoostReg/assets/29518499/011aff10-64ce-4bff-8275-a18a579ecbc8)

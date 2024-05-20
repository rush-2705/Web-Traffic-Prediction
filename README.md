# Web-Traffic-Prediction


Website traffic prediction is the process of forecasting the number of visitors to a website over time using historical web traffic data. Websites monitor and collect data of incoming and outgoing traffic on a particular website. Many times, there is a sudden surge of user activity on a website due to certain reasons. For such reasons website companies need to allocate more server resources to handle this surge in traffic to avoid a website crash. The resource allocation must be dynamic and should be based on multiple factors. For handling this dynamic allocation, we can use the data collected by the websites and model the data using some data modeling techniques to forecast the number of users on a particular website on a particular day. In this project we will be using the dataset containing websites and their number of daily page hits on certain dates. Accurate website traffic prediction is important for website companies to allocate server resources effectively, optimize website performance, and provide better user experience, leading to increased revenue.



Description of data: The dataset contains around 145,000 time series representing the number of daily views of different Wikipedia articles from July 1st, 2015 to December 31st, 2016. Each time series is associated with the name of the article and the type of traffic it represents, such as all, mobile, desktop, or spider. However, the database did not distinguish between zero traffic values and missing values, so a missing value could mean either zero traffic or unavailable data for that day. That’s why data preprocessing was necessary.



In this project, we explored various time series forecasting models including AR, ARIMA, Prophet, LSTM and XGBoost to model web traffic data and selected the most appropriate one based on their performance. A brief description of the models used is as follows:
    
1. AR (Autoregressive) Model: This model uses past observations to predict future observations. It is a simple model that assumes that future values are dependent on previous values.
2. ARIMA (Autoregressive Integrated Moving Average) Model: This model is similar to the AR model but also takes into account the moving average in the data.
3. Prophet: This is a model developed by Facebook that uses time series decomposition to model trends, seasonality, and holidays. It can handle missing values and outliers.
4. LSTM (Long Short-Term Memory) Model: This is a type of neural network that is able to remember previous inputs and their relationships to each other, allowing it to model complex patterns in the data.
5. XGBoost: This is a type of decision tree model that is optimized for accuracy and speed. It works by creating a series of trees that iteratively correct the errors of previous trees, ultimately producing a highly accurate prediction.


Results: After evaluating the performance of various time series forecasting models, we found that LSTM had the lowest Symmetric Mean Absolute Percentage Error (SMAPE) and was the most accurate model in predicting web traffic.

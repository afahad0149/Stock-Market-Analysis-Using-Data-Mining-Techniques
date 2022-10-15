# Stock-Market-Analysis-Using-Data-Mining-Techniques
Analysis and Prediction of Dhaka Stock Exchange Broad Index trends over the last 10 years.

## Objective
Given how complex and volatile the stock market is, experts have long been interested in predicting price movements. Intrinsic volatility in stock market across the globe makes the task of prediction challenging. To ensure minimal investment risk, market risk, which is strongly correlated with forecasting errors, needs to be reduced. Machine learning and Deep learning is used as popular tool for analysis and prediction for accurate result. In this regard, we different deep learning techniques to observe the better estimation of our selected dataset.

## Python libraries used
- Matplotlib
- Seaborn
- scikit-learn
- Keras and TensorFlow

## Experimental Data
For our project, we collected the historical data DSE Broad Index (DSEX) for the last 10 years since its inception. The DSEX, which represents approximately 97% of the overall stock market capitalization, is the Exchange's Broad Index (also known as a Benchmark Index because it displays the precise price movement of the listed companies).
The total number of data points was 2,262 with the features: Date, Opening Price, High Price, Low Price, Closing Price, Volume, and Rate of Change. As values of Volume were missing for almost all data points and  Rate of Change depended on High Price and Low Price, they were dropped. For the rest of the features, data visualization was performed using Python 3 libraries Matplotlib and Seaborn.

## Data Preprocessing and Feature Selection
Each values of the data was converted into real numbers from strings and due to the wide range of values, features were scaled using min max scaling to keep their values between 0 and 1. As discussed previously, the target feature was the Closing Price. The input features were divided into three sets: {Opening Price}, {High Price, Low Price}, and {Opening Price, High Price, and Low Price}. Then train-test split was performed where 70% of the data were used for training and the remaining 30% for testing. 

## Machine Learning Models Used
- Linear Regressor
- Support Vector Regressor
- Decision Tree Regressor
- Random Forest Regressor
- Artificial Neural Network
- Long Short Term Memory (LSTM)

## Performance Measure
To measure the performance of each of the models more rigorously, we employed 10 folds cross validation for each of the models trained with each feature sets:  {Opening Price}, {High Price, Low Price}. Then we calculated the mean and the standard deviation of each of the distributions obtained from the Mean Squared Error of each 10-folds cross validation.

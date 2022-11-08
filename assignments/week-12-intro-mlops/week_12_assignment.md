Link to the **stock-predictor** repo: 

[https://github.com/yinghu-math/stock-predictor]

**Essay questions:** 

**Q1:** How does the Prophet Algorithm differ from an LSTM? Why does an LSTM have poor performance against ARIMA and Prophet for Time Series?

**Ans:** Prophet Algorithm is specifically designed for the prediction of business time series. The model takes into account the seasonality of the business data. 

Unlike time series-specific models such as ARIMA and Prophet, LSTM is a general RNN-based deep learning layer, and its usage is not restricted to time series. However, a deep learning model using LSTM needs a large amount of data to train. When applied to a small dataset, it tends to be overfitted. 

[Here](https://neptune.ai/blog/arima-vs-prophet-vs-lstm) is a post that contains the experimental data of these three models. 


**Q2:** What is exponential smoothing and why is it used in Time Series Forecasting?

**Ans:**  Exponential smoothing can be used as a forecasting model. It predicts the new values from the weighted sum of all past observations, where the weight of an observation exponentially decays as the observation get older. 

**Q3:** What is stationarity? What is seasonality? Why Is Stationarity Important in Time Series Forecasting?

**Ans:** The stationarity of a time series refers to that the pattern of the time series doesn't change over time.  This is an important property for prediction since most models are based on learning patterns of past data to predict the future.  Seasonality of a time series refers to that the data experiences regular and predictable changes that recur every calendar year, like retail sales data.


**Q4:** How is seasonality different from cyclicality? Fill in the blanks:


**Ans:** Seasonality is predictable, whereas cyclicality is not.




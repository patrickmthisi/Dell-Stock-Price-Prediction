# Dell-Stock-Price-Prediction
The dataset consists of Dell's stock prices. For more information  about the data used in this project, refer to:

https://www.kaggle.com/datasets/zongaobian/microsoft-stock-data-and-key-affiliated-companies?select=DELL_daily_data.csv.

## Project description and objectives:

This comprehensive project aims to tease out various Holt-Winters configurations to identify which ones yield superior prediction performance for Dell's daily stock prices. This notebook is an extensive demonstration of a Holt-Winters ETS-based time series forecasting approach for Dell's stock prices, encompassing time series analysis, visualization, and performance evaluation using RMSE.

The following essential time series forecasting concepts are explored in this project:
1. Holt-Winters Modelling: The ETS (Error, Trend, Seasonality) model is utilized for forecasting. This process involves determining the optimal ETS parameters for level, trend, dampening, and seasonal effects, achieved through an automated search of historical data to identify the best parameters.
2. Rolling Forecast: 
    - Once the model is fitted, a rolling forecast method is applied, allowing for predictions to be made one step ahead. The model is updated iteratively using actual values.
3. Model Evaluation:
    - The predicted values are compared to the actual values from the validation set.
    - The Root Mean Squared Error (RMSE) is the metric used to assess the model's performance.
    - Final predictions alongside the actual validation data are visualized.    
4. Next Steps: The project also highlights potential future enhancements, such as exploring additional time series forecasting models. These may include classical approaches like SARIMA and more advanced methodologies involving CNNs and LSTMs.

## Conclusion and further work
In this comprehensive project, we developed an Exponential Smoothing (ETS) model to forecast Dell's stock price. We compared the performance of the ETS model against a naive model, which served as our baseline model. The ETS model achieved a Root Mean Square Error (RMSE) of 4.168, which is closely aligned with the performance of the naive model. The top five ETS models exhibited only marginal differences, with RMSE values ranging from 4.168 to 4.173. In contrast, the top five naive models displayed greater variability, with RMSE values spanning from 4.169 to 5.837.

Ultimately, we decided to proceed with the ETS model, reporting impressive performance using the out-of-sample validation dataset. The residuals of the model closely approximated a Gaussian distribution, as illustrated by the Q-Q plot. However, the overall performance of the ETS model did not meet our expectations for this dataset. As a result, future work could consider exploring other classical time-series models, such as SARIMA, or adopting advanced deep learning techniques like Convolutional Neural Networks (CNN) and Long Short-Term Memory (LSTM) networks.

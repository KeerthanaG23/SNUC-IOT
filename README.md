# Time series from IoT devices: anomaly detection and forecast 

## 1.Background
A young couple wants to buy a house with connected devices and solar panels. The owner has collected and shared data from IoT devices. 

Expected goals for this project: 
<br>
- Illustrate trends of energy consumption and generation

- Detect eventual appliance anomalies that may have boosted the consumption
- Predict future consumption 
Time series data from IoT devices can be challenging to analyze due to their high volume, velocity, and variety. However, there are several techniques that can be used for anomaly detection and forecast of IoT time series data:

## Anomaly Detection:
Statistical methods such as mean, median, and standard deviation can be used to identify outliers or anomalies in the data.


Machine learning techniques such as clustering, decision trees, and neural networks can also be applied to detect anomalies.


Time series decomposition methods such as seasonal decomposition of time series (STL) can help separate the trend, seasonal, and residual components of the time series data, making it easier to identify anomalies in the residual component.
## Forecasting:
Autoregressive integrated moving average (ARIMA) models can be used to forecast the future values of a time series based on its past values.
Machine learning algorithms such as random forest, gradient boosting, and neural networks can also be applied to make accurate predictions.
Deep learning models such as long short-term memory (LSTM) and gated recurrent units (GRU) can capture long-term dependencies in the time series data and provide accurate predictions.
It's important to note that the choice of the method depends on the nature of the IoT data and the specific problem being addressed. It's also important to continually monitor and update the anomaly detection and forecasting models to ensure their accuracy and effectiveness over time.

## 2. The data

The smart-home dataset available on Kaggle

https://www.kaggle.com/datasets/taranvee/smart-home-dataset-with-weather-information

a 130MB csv file with several features including weather, power generated, and consumption by appliance detector.


## 3. The model outcome

Application of CUSUM method for anomaly detection showed that there were some consumption spikes, correlated to the weather but no points of steady increase. 

Models built with LightGBM can predict future energy consumption when weather information was added to the simple time information. 



## 4. Conclusions

- Consumption is high during the night, and increases significantly during hot months in the summer. This is likely due to air conditioning, house insulation may be improved.

- Almost no solar energy produced in the morning: panels orientation must be checked.

- Home appliances work well, no evident faults detected from trends anomaly.

## AS I HAVE A TROUBLE IN INSTALLING THE KATS LIBRARY I WAS NOT ABLE TO  FORECAST 
WILL UPDATE SOON


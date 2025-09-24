# RUB-YAN-predict
A project aimed at analyzing and predicting the exchange rate of the RUB/YAN currency pair using a combination of SARIMAX, HMM, and LSTM models.

### Analysis and Forecasting

For data analysis and forecasting, we leveraged the following Python libraries: **NumPy**, **Pandas**, **scikit-learn**, **Matplotlib**, **Statsmodels**, **TensorFlow**, and **hmmlearn**.

Historical data analysis—conducted in spring 2025—revealed that by mid-June 2025, the exchange rate would decline to approximately **11 RUB per CNY**. The actual observed rate closely matched this prediction, settling in the range of **10.8–11 RUB per CNY**.

#### Ensemble Model Performance Metrics:
- **MSE**: 0.0326  
- **MAE**: 0.1412  
- **MAPE**: 1.20%  
- **R²**: 0.726  

These metrics indicate strong predictive performance:  
- The low **MAE** suggests minimal average absolute error, confirming high accuracy for short-term forecasts.  
- The low **MSE** implies the absence of significant outliers, reflecting robustness in longer-term predictions.  
- The **MAPE** of just over 1% demonstrates low relative (percentage) error, further validating the model's reliability.

#### Ensemble Composition:
- **SARIMAX**: 40%  
- **Hidden Markov Model (HMM)**: 30%  
- **LSTM**: 30%  

The balanced combination of statistical, probabilistic, and deep learning approaches enables the ensemble to capture diverse patterns in the time series, resulting in accurate and stable forecasts.

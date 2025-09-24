# RUB-YAN-predict
A project aimed at analyzing and predicting the exchange rate of the RUB/YAN currency pair using a combination of SARIMAX, HMM, and LSTM models.


### Analysis and Forecasting

For data analysis and forecasting, we leveraged the following Python libraries: **NumPy**, **Pandas**, **scikit-learn**, **Matplotlib**, **Statsmodels**, **TensorFlow**, and **hmmlearn**.

Historical data analysis—conducted in spring 2025—revealed that by mid-June 2025, the exchange rate would decline to approximately **11 RUB per CNY**. The actual observed rate closely matched this prediction, settling in the range of **10.8–11 RUB per CNY**.

#### Ensemble Model Performance Metrics:
- **MSE**: 0.0326  
- **MAE**: 0.1412  
- **MAPE**: 1.20%  
- **R² (Coefficient of Determination)**: 0.726  

**Interpretation of metrics:**  
- The low **Mean Absolute Error (MAE)** indicates that, on average, the model’s predictions deviate from the true values by only about **0.14 RUB**, which is excellent for short-term forecasting.  
- The low **Mean Squared Error (MSE)** suggests that large errors (outliers) are rare, confirming the model’s stability over longer horizons.  
- The **Mean Absolute Percentage Error (MAPE)** of **1.20%** reflects very low relative error—meaning predictions are typically within ~1% of actual values.  
- The **R² score of 0.726** means that approximately **72.6% of the variance** in the exchange rate is explained by the model. In other words, the model captures the majority of the underlying patterns in the data, which is considered strong performance for a real-world financial time series.

#### Ensemble Composition:
- **SARIMAX**: 40%  
- **Hidden Markov Model (HMM)**: 30%  
- **LSTM**: 30%  

This hybrid ensemble combines the strengths of classical statistical modeling (SARIMAX), probabilistic state-based forecasting (HMM), and deep learning (LSTM). The result is a robust, adaptive system capable of capturing linear trends, regime shifts, and complex nonlinear dynamics—leading to accurate and reliable exchange rate predictions.

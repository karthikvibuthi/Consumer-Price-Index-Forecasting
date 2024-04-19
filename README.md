# Consumer-Price-Index-Forecasting
In this project I have analyzed time series data of US Consumer Price Index to model and forecast for out of sample data.

### Project Description

#### Goal
The goal of this project is to forecast the US core Consumer Price Index (CPI) excluding Food and Energy (CPILFESL) using time series analysis techniques.

#### Data
The dataset used is sourced from the Federal Reserve Economic Data (FRED) provided by the St. Louis Fed. It represents the Consumer Price Index excluding Energy and Food, which are known to be volatile components.

![image](https://github.com/karthikvibuthi/Consumer-Price-Index-Forecasting/assets/141452458/168b0df2-1358-42e3-b94b-eb0051b787fc)

#### Project Components
1. **Year-over-Year Percentage Change Calculation**: Calculated the year-over-year percentage change of the CPI series.
2. **Time Series Plots**: Created time series plots to visualize the observed non-seasonal and detrended data with cyclic patterns.

  ![image](https://github.com/karthikvibuthi/Consumer-Price-Index-Forecasting/assets/141452458/9de86d21-cf72-447e-a58e-17cd0c98be32)
  

3. **Model Selection**: Based on the Autocorrelation Function (ACF) and Partial Autocorrelation Function (PACF), determined the optimal number of ARIMA terms as \(p=2\), \(d=1\), and \(q=1\).
4. **Data Splitting**: Split the data into training and test sets, using the last 12 months as the test series.
5. **Model Fitting**: Fitted ARIMA, exponential smoothing, and naive models to the training data.

 ![image](https://github.com/karthikvibuthi/Consumer-Price-Index-Forecasting/assets/141452458/26ca011f-4c0e-4068-b6ca-968eed7000f3)

6. **Model Evaluation**: Inspected the ARIMA model report and evaluated the performance metrics including Mean Error (ME), Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), Mean Percentage Error (MPE), Mean Absolute Percentage Error (MAPE), Mean Absolute Scaled Error (MASE), Root Mean Squared Scaled Error (RMSSE), and Autocorrelation of Residuals (ACF1).

 ![image](https://github.com/karthikvibuthi/Consumer-Price-Index-Forecasting/assets/141452458/b3c4fa1c-406f-47f3-a3d9-43f4035f10a3)

7. **Best Model Selection**: Chose the best model based on performance metrics, with Auto Arima being the preferred model.
8. **Model Retraining and Forecasting**: Retrained the best model and forecasted the CPI for the next 12 months.
![image](https://github.com/karthikvibuthi/Consumer-Price-Index-Forecasting/assets/141452458/a418ca50-fb88-4045-bbde-d7a7634272ce)

### Conclusion
The project successfully applied time series analysis techniques to forecast the US core CPI, providing valuable insights for decision-making and future planning.

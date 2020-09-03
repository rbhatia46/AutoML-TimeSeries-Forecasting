# AutoML-TimeSeries-Forecasting
Use of [ATSPy](https://github.com/firmai/atspy), a library to automate time series forecasting, using multiple models and ensembles.

#### Automated Models

1. ```ARIMA``` - Automated ARIMA Modelling
1. ```Prophet``` - Modeling Multiple Seasonality With Linear or Non-linear Growth
1. ```HWAAS``` - Exponential Smoothing With Additive Trend and Additive Seasonality
1. ```HWAMS``` - Exponential Smoothing with Additive Trend and Multiplicative Seasonality
1. ```PYAF``` - Feature Generating Model (slow and underforms)
1. ```NBEATS``` -  Neural basis expansion analysis (now fixed at 20 Epochs)
1. ```Gluonts``` - RNN-based Model (now fixed at 20 Epochs)
1. ```TATS``` - Seasonal and Trend no Box Cox
1. ```TBAT``` - Trend and Box Cox
1. ```TBATS1``` - Trend, Seasonal (one), and Box Cox
1. ```TBATP1``` - TBATS1 but Seasonal Inference is Hardcoded by Periodicity
1. ```TBATS2``` - TBATS1 With Two Seasonal Periods

#### Why AtsPy?

1. Implements all time series models in a unified manner by simply running ```AutomatedModel(df)```.
2. Automatically identify the seasonalities in your data using singular spectrum analysis, periodograms, and peak analysis.
3. Identifies and makes accessible the best model for your time series using in-sample validation methods.  
4. Combines the predictions of all these models in a simple (average) and complex (GBM) ensembles for improved performance.
5. Where appropriate models have been developed to use GPU resources to speed up the automation process.

A blog post on Atspy : https://analyticsindiamag.com/hands-on-guide-to-atspy-for-automating-the-time-series-forecasting/

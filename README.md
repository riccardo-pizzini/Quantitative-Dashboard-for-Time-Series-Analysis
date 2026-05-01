# Quant Dashboard

**Quant Dashboard** is a MATLAB App Designer application designed for financial time series analysis, volatility modelling, risk forecasting and statistical diagnostics.

The app allows users to download historical market data, analyze asset returns, inspect autocorrelation structures, estimate ARIMA/GARCH models, forecast volatility and evaluate downside risk through Value at Risk backtesting.

---

## Overview

Quant Dashboard provides an intuitive interface for quantitative financial analysis.

Instead of running separate scripts or manually inspecting outputs from the MATLAB command window, the app organizes the entire workflow into a graphical dashboard.

The project is mainly focused on:

- Financial return analysis
- Time series diagnostics
- Volatility modelling
- Risk forecasting
- Distribution and tail-risk analysis

The goal of the application is to make quantitative finance tools easier to use, interpret and visualize.

---

## Main Features

### Market Data Analysis

- Download historical price data for a selected asset
- Select custom date ranges
- Display historical price dynamics
- Compute daily and annualized return statistics

### Return Dynamics

- Calculate log returns
- Visualize return behavior over time
- Analyze mean return and standard deviation
- Compare daily and annualized volatility

### Time Series Diagnostics

- Augmented Dickey-Fuller test for stationarity analysis
- ACF and PACF analysis on returns
- ACF and PACF analysis on squared returns
- Ljung-Box test on squared residuals
- Jarque-Bera test for normality assessment

### ARIMA Modelling

- Automatic ARIMA order selection
- Residual analysis
- Diagnostic plots for model validation
- Evaluation of autocorrelation in residuals

### GARCH Volatility Modelling

- Detection of volatility clustering
- Automatic GARCH model selection
- Volatility forecasting
- Rolling volatility analysis
- Confidence bands for forecast interpretation

### Risk Forecasting

- Value at Risk estimation
- VaR backtesting
- Violation count analysis
- Comparison between observed and expected violation rates
- Risk interpretation based on the selected confidence level

### Distribution and Tail-Risk Analysis

- Return distribution visualization
- Tail-risk inspection
- Normality comparison
- Statistical interpretation of extreme observations

---

## App Structure

The application is organized into five main tabs:

1. **Dashboard**  
   General overview of the selected asset, price dynamics and summary statistics.

2. **Returns Dynamics**  
   Analysis of asset returns, volatility and return behavior over time.

3. **Residuals**  
   ARIMA residual diagnostics, autocorrelation checks and model validation.

4. **Risk Forecasting**  
   GARCH volatility forecast, rolling volatility and Value at Risk backtesting.

5. **Distribution & Tail Risks**  
   Distribution analysis, normality testing and tail-risk interpretation.

---

## Screenshots

Add your app screenshots here.

![Dashboard Screenshot](images/dashboard.png)

![Returns Dynamics Screenshot](images/returns-dynamics.png)

![Residuals Screenshot](images/residuals.png)

![Risk Forecasting Screenshot](images/risk-forecasting.png)

![Distribution and Tail Risks Screenshot](images/distribution-tail-risk.png)

---

## Recommended Folder Structure

```text
quant-dashboard/
│
├── README.md
├── LICENSE
│
├── src/
│   ├── QUANT_DASHBOARD.mlapp
│   ├── firstcalculation.m
│   └── getYahoo.m
│
├── images/
│   ├── dashboard.png
│   ├── returns-dynamics.png
│   ├── residuals.png
│   ├── risk-forecasting.png
│   └── distribution-tail-risk.png
│
└── docs/
    └── methodology.md
```

---

## Technologies Used

- MATLAB
- MATLAB App Designer
- Econometrics Toolbox
- Statistics and Machine Learning Toolbox
- Financial time series analysis
- ARIMA modelling
- GARCH volatility modelling
- Value at Risk backtesting

---

## Methodology

Quant Dashboard follows a standard quantitative finance workflow.

First, the app retrieves historical price data for the selected asset and computes log returns.  
Then, descriptive statistics are calculated to summarize the behavior of the return series.

Stationarity is assessed through the Augmented Dickey-Fuller test.  
Autocorrelation is analyzed using ACF and PACF plots, both on returns and squared returns.

If volatility clustering is detected, the app estimates a GARCH model and produces a volatility forecast.  
The estimated volatility is then used to support downside risk analysis through Value at Risk backtesting.

The app also provides automatic comments and interpretations to help users understand the statistical results.

---

## Example Use Cases

Quant Dashboard can be used to:

- Analyze the historical behavior of a stock, ETF or market index
- Study the volatility of a financial asset
- Detect volatility clustering
- Evaluate whether a GARCH model is useful
- Forecast future volatility
- Backtest Value at Risk estimates
- Compare statistical properties across different assets
- Support academic projects in quantitative finance and econometrics

---

## Requirements

To run the application, you need:

- MATLAB
- MATLAB App Designer
- Econometrics Toolbox
- Statistics and Machine Learning Toolbox

Depending on the data download method used in the app, an external script or connection to a financial data source may also be required.

---

## Installation

Clone the repository:

```bash
[git clone https://github.com/your-username/quant-dashboard.git](https://github.com/riccardo-pizzini/Quantitative-Dashboard-for-Time-Series-Analysis)
```

Open the project in MATLAB and run the `.mlapp` file:

```matlab
open('src/QUANT_DASHBOARD.mlapp')
```

Then click **Run** inside MATLAB App Designer.

---

## Usage

1. Insert the ticker of the asset you want to analyze.
2. Select the start and end dates.
3. Choose the forecast horizon.
4. Select the confidence level for risk analysis.
5. Run the calculation.
6. Explore the results across the different tabs.

---

## Project Status

This project is currently under development.

Planned improvements may include:

- Support for multiple assets
- Portfolio-level analysis
- Exportable reports
- Additional risk measures
- Improved model comparison
- Enhanced user interface
- More flexible data source integration

---

## Disclaimer

This project is developed for educational and research purposes only.

The results produced by the application should not be considered financial advice, investment recommendations or trading signals.  
Financial markets involve risk, and quantitative models are based on assumptions that may not always hold in real market conditions.

---

## Author

Developed by **Riccardo Pizzini**

You can connect with me on:

- LinkedIn: https://www.linkedin.com/in/riccardo-pizzini-a84078249/
- GitHub: https://github.com/riccardo-pizzini

---

## License

This project is released under the MIT License.

See the `LICENSE` file for more details.

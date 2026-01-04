# Measles Time Series Analysis (2010–2024)

## Overview
- Comprehensive time series analysis of notified measles cases (2010–2024)
- Implemented in **R** using classical and modern forecasting methods
- Focus on **trend, seasonality, stationarity, and model comparison**
- Designed for **public health surveillance and early warning applications**

---

## Objectives
- Describe long-term and short-term measles trends
- Identify and characterise seasonal patterns
- Assess stationarity and temporal dependence
- Decompose the series using multiple techniques
- Compare forecasting performance across models

---

## Data
- Temporal resolution: **Monthly**
- Study period: **2010–2024**
- Data type: **Univariate time series (case counts)**
- Source: **Routine surveillance notifications**
- Note: Raw data not included due to confidentiality

---

## Methods

### Exploratory & Diagnostic Analysis
- Yearly and weekly trend visualisation
- Seasonal, polar, and subseries plots
- Spectral analysis (Periodogram, FFT)
- Autocorrelation and partial autocorrelation (ACF, PACF)
- Ljung–Box test for serial correlation
- Stationarity testing (ADF)

### Decomposition Techniques
- Classical decomposition (additive, multiplicative)
- X-11 decomposition
- SEATS decomposition
- STL decomposition (robust, periodic seasonality)

### Forecasting Models
- ARIMA
- SARIMA
- STL + ARIMA
- Exponential Smoothing (ETS)
- Holt–Winters
- TBATS

### Model Evaluation
- Train–test split (training: 2010–2022, testing: 2023–2024)
- Accuracy metrics:
  - RMSE
  - MAE
  - MSE
  - MAPE
- Visual comparison of observed vs forecast values

---

## Key Findings
- Measles incidence exhibits **weak but persistent seasonality**
- Seasonal peaks recur annually with intra-year fluctuations
- Additive decomposition is more appropriate than multiplicative
- Differencing confirms true seasonality rather than trend artefact
- SARIMA and STL+ARIMA generally provide superior forecast accuracy

---

## Software & Packages
- R (≥ 4.0)
- tidyverse
- ggplot2
- fpp2
- forecast
- seasonal
- tseries
- urca

---

## Repository Structure
- `scripts/` – R scripts for analysis and modelling
- `README.md`

---

## Intended Use
- Epidemiological time series training
- Public health surveillance analysis
- Forecasting method comparison
- Reference for postgraduate public health research

---

## SWOT Analysis

### Strengths
- Comprehensive and structured time series workflow
- Multiple decomposition and forecasting methods
- Objective model comparison using standard accuracy metrics
- Strong alignment with public health surveillance practice

### Weaknesses
- Univariate analysis without explanatory covariates
- Potential under-reporting and reporting delay bias
- Structural breaks not explicitly modelled

### Opportunities
- Extension to multivariate or regression-based time series
- Integration of vaccination coverage or climate variables
- Development of outbreak early-warning thresholds
- Deployment into routine surveillance dashboards

### Threats
- Changes in notification practices over time
- Policy or outbreak response effects causing structural breaks
- Reduced predictive performance during atypical epidemic years

---

## Citation
If used for academic or policy work, please cite:

Sha’ari AZ. *Measles Time Series Analysis (2010–2024)*. GitHub repository.

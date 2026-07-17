# Wikipedia Traffic Forecasting using Time Series Analysis

Forecasting daily Wikipedia page traffic using statistical and machine learning time series models to support advertisement planning, capacity management, and user demand forecasting.

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Time Series](https://img.shields.io/badge/Time%20Series-Forecasting-orange)
![SARIMAX](https://img.shields.io/badge/SARIMAX-Model-success)
![License](https://img.shields.io/badge/License-MIT-green)

---

# Overview

Accurate traffic forecasting enables organizations to anticipate user demand, optimize infrastructure, improve resource allocation, and support strategic planning.

This project develops an end-to-end forecasting pipeline to predict daily Wikipedia page views using classical and modern time series forecasting techniques including **ARIMA, SARIMAX, and Prophet**.

---

# Business Problem

Millions of users access Wikipedia every day, resulting in highly dynamic traffic patterns influenced by seasonality, trends, holidays, and special events.

Reliable traffic forecasting helps organizations:

- Optimize server capacity
- Improve content delivery performance
- Plan digital advertising campaigns
- Forecast resource utilization
- Reduce operational costs

---

# Project Objectives

- Forecast future Wikipedia page traffic
- Compare multiple forecasting models
- Identify seasonality and trends
- Evaluate model performance using forecasting metrics
- Generate actionable business insights

---

# Dataset

- **Source:** Wikipedia Web Traffic Time Series Dataset
- **Records:** 145,000+ Wikipedia pages
- **Frequency:** Daily
- **Forecast Horizon:** 60 Days

---

# Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Statsmodels
- Prophet
- Scikit-learn

---

# Project Workflow

```
Data Collection
        │
        ▼
Data Cleaning
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Trend Analysis
        │
        ▼
Stationarity Testing
        │
        ▼
Feature Engineering
        │
        ▼
Model Development
        │
        ▼
Model Evaluation
        │
        ▼
Forecast Generation
```

---

# Exploratory Data Analysis

Performed extensive exploratory analysis including:

- Missing value analysis
- Trend visualization
- Seasonal decomposition
- Rolling averages
- Traffic distribution
- Outlier detection

---

# Data Preprocessing

- Missing value treatment
- Time index conversion
- Resampling
- Log transformation
- Train-test split

---

# Statistical Analysis

Performed statistical tests including:

- Augmented Dickey-Fuller (ADF) Test
- Seasonal decomposition
- Autocorrelation Function (ACF)
- Partial Autocorrelation Function (PACF)

These analyses were used to determine model parameters and confirm stationarity.

---

# Forecasting Models

The following forecasting models were evaluated:

- Naïve Forecast
- Moving Average
- ARIMA
- SARIMAX
- Facebook Prophet

SARIMAX delivered the best forecasting performance.

---

# Best Model

**SARIMAX (2,1,2)(2,1,0,7)**

The selected model effectively captured:

- Trend
- Weekly seasonality
- Temporal dependencies

---

# Model Performance

| Metric | Score |
|---------|--------|
| MAPE | 5.1% |
| RMSE | 385.38 |

---

# Forecast Visualization

The project generates:

- Historical Traffic Trends
- Forecast vs Actual
- Confidence Intervals
- Seasonal Components
- Residual Analysis

(Add screenshots in the `images/` folder.)

---

# Business Insights

- Weekly seasonality significantly influences traffic.
- SARIMAX outperformed ARIMA and Prophet for this dataset.
- Accurate forecasting enables better infrastructure planning.
- Demand forecasting can improve advertisement scheduling and resource allocation.

---

# Repository Structure

```
wikipedia-traffic-forecasting
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│
├── src/
│
├── models/
│
├── reports/
│
├── images/
│
├── requirements.txt
│
├── README.md
│
└── LICENSE
```

---

# Skills Demonstrated

- Time Series Forecasting
- ARIMA
- SARIMAX
- Prophet
- Forecast Evaluation
- Statistical Analysis
- Feature Engineering
- Exploratory Data Analysis
- Data Visualization
- Predictive Analytics

---

# Future Improvements

- Automate retraining using Airflow
- Deploy forecasting API using FastAPI
- Create interactive dashboard using Streamlit
- Experiment with LSTM and Transformer-based forecasting models
- Integrate MLflow for experiment tracking

---

# Installation

```bash
git clone https://github.com/<your-username>/wikipedia-traffic-forecasting.git

cd wikipedia-traffic-forecasting

pip install -r requirements.txt
```

---

# Results

The forecasting pipeline achieved:

- **MAPE:** 5.1%
- **RMSE:** 385.38

The SARIMAX model consistently outperformed baseline forecasting methods by effectively capturing trend and seasonal patterns.

---




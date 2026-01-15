# Stock Market Analysis & Forecasting  
_Dissertation Project (Applied Data Science & Time Series Analysis)_

## Overview
This project presents an **applied stock market analysis and forecasting study** developed as part of my postgraduate dissertation.  
It combines **statistical time-series modelling, machine learning techniques, and visual analytics** to support **data-driven financial decision-making**.

The focus is on building **interpretable, reproducible forecasting pipelines** and evaluating their real-world performance using industry-standard error metrics.

---

## Project Objectives
- Analyse historical stock price behaviour and volatility
- Compare classical and modern forecasting approaches
- Evaluate predictive performance using multiple accuracy metrics
- Demonstrate how forecasting insights can support financial planning and risk assessment

---

## Methods Used
The project follows a structured analytical pipeline:

### 1. Exploratory Data Analysis
- Price trends and returns analysis  
- Volatility inspection  
- Seasonal and trend decomposition (STL)

### 2. Forecasting Models
- **ARIMA** (AutoRegressive Integrated Moving Average)
- **Facebook Prophet** (additive time-series model with trend and seasonality)

### 3. Unsupervised Learning
- **PCA (Principal Component Analysis)** for dimensionality reduction
- **K-Means clustering** to identify volatility and behaviour regimes

### 4. Evaluation Metrics
Models were evaluated using:
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Percentage Error (MAPE)
- Forecast Accuracy (%)

---

## Results Summary

| Model    | MAE | RMSE | MAPE | Accuracy |
|--------|-----|------|------|----------|
| ARIMA  | 4.95 | 5.89 | 8.93% | 91.07% |
| Prophet | **3.10** | **3.76** | **5.95%** | **94.05%** |

**Key findings:**
- Prophet consistently outperformed ARIMA across all evaluation metrics
- Lower MAPE indicates improved robustness to volatility
- Forecast intervals provided clearer uncertainty estimation
- Clustering revealed distinct volatility regimes useful for risk profiling

---

## Decision & Business Interpretation
The forecasting outputs enable:
- Improved short-term price expectation modelling
- Enhanced volatility awareness for risk-sensitive decisions
- Comparative assessment of forecasting reliability
- Scenario-based planning rather than reactive analysis

This demonstrates how **time-series forecasting can move beyond prediction to support strategic financial decision-making**.

---

## Reproducibility

### How to Run
1. Open `complete_dissertation.Rmd` in RStudio
2. Install required packages (first run):
   ```r
   install.packages(c(
     "tidyverse",
     "dplyr",
     "ggplot2",
     "plotly",
     "forecast",
     "prophet",
     "cluster",
     "factoextra"
   ))
 3. Knit the RMarkdown file to reproduce the full analysis and outputs

## Project Artefacts

 complete_dissertation.Rmd — full reproducible analysis pipeline

 stockpriceanalysis.pdf — final dissertation report

assets/ — visual outputs (forecast plots & clustering)

## Data Note

This project uses historical financial market data for academic analysis.
The focus is on methodology, evaluation, and decision insight, rather than proprietary trading signals.

## Author Note

This project reflects my interest in applied analytics, forecasting, and decision-oriented data science, bridging statistical modelling with practical business and financial insight.

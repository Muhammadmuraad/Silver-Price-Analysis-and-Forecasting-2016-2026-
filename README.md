# Silver Price Analysis and Forecasting Project

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 📊 Project Overview

This project provides a comprehensive analysis of silver prices over the past 10 years (2016-2026), including exploratory data analysis (EDA), machine learning models, and price forecasting until March 2026.

## 🎯 Objectives

- Analyze 10 years of silver price historical data
- Perform comprehensive exploratory data analysis
- Build and compare multiple ML forecasting models
- Forecast silver prices until March 2026
- Identify factors driving 2026 price movements
- Provide investment insights and recommendations

## 📁 Project Structure

```
silver price/
├── silver_data.csv                    # Historical silver price data
├── silver_price_forecast.csv          # Forecasted prices
├── silver_price_analysis.ipynb        # Main analysis notebook
├── requirements.txt                   # Python dependencies
├── setup_env.bat                      # Environment setup script
├── create_notebook.py                 # Notebook generator script
├── README.md                          # This file
└── KAGGLE_DESCRIPTION.md             # Kaggle dataset description
```

## 🚀 Quick Start

### Prerequisites

- Python 3.8 or higher
- pip package manager

### Installation

1. **Clone or download this repository**

2. **Run the setup script** (Windows):
   ```bash
   setup_env.bat
   ```

   Or manually:
   ```bash
   python -m venv venv
   venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. **Generate the Jupyter notebook**:
   ```bash
   python create_notebook.py
   ```

4. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook silver_price_analysis.ipynb
   ```

## 📊 Dataset Information

### Source
- **Data Provider**: Yahoo Finance (yfinance)
- **Ticker Symbol**: SI=F (Silver Futures)
- **Time Period**: 2016 - 2026 (10 years)
- **Frequency**: Daily

### Features
- **Date**: Trading date
- **Open**: Opening price
- **High**: Highest price of the day
- **Low**: Lowest price of the day
- **Close**: Closing price
- **Volume**: Trading volume
- **Adj Close**: Adjusted closing price

## 🤖 Machine Learning Models

Four different models were tested and compared:

1. **LSTM (Long Short-Term Memory)**
   - Deep learning model for sequential data
   - Captures long-term dependencies
   - 3-layer architecture with dropout

2. **Facebook Prophet**
   - Automated time series forecasting
   - Handles seasonality and trends
   - Robust to missing data and outliers

3. **ARIMA**
   - Classical statistical approach
   - Autoregressive Integrated Moving Average
   - ARIMA(5,1,2) configuration

4. **XGBoost**
   - Gradient boosting with time series features
   - Technical indicators as features
   - Best for non-linear patterns

### Model Evaluation Metrics

- **RMSE**: Root Mean Squared Error
- **MAE**: Mean Absolute Error
- **MAPE**: Mean Absolute Percentage Error
- **R² Score**: Coefficient of determination

## 📈 Key Findings

### 2026 Price Movement Factors

1. **Industrial Demand Growth**
   - Solar energy sector expansion
   - Electric vehicle production
   - 5G infrastructure deployment

2. **Economic Factors**
   - Inflation hedging demand
   - Geopolitical tensions
   - Supply chain constraints

3. **Market Dynamics**
   - Mining supply limitations
   - Investment demand (ETFs)
   - USD strength/weakness

### Future Projections

- Detailed forecasts until March 2026
- Confidence intervals provided
- Multiple scenarios (conservative, base, optimistic)
- Risk factors identified

## 📊 Visualizations Include

- Price trends and patterns
- Candlestick charts
- Technical indicators (RSI, MACD, Bollinger Bands)
- Seasonality decomposition
- Volume analysis
- Model performance comparisons
- Forecast with confidence intervals

## 💡 Usage for Kaggle

This project is designed to be uploaded to Kaggle. All required files are included:

1. Upload `silver_data.csv` and `silver_price_forecast.csv` as a dataset
2. Create a new notebook and upload `silver_price_analysis.ipynb`
3. Run the notebook to reproduce all results
4. Use `KAGGLE_DESCRIPTION.md` for dataset description

### Potential Use Cases on Kaggle

- Time series forecasting practice
- Financial data analysis learning
- ML model comparison studies
- Investment strategy backtesting
- Economic research and analysis

## 🛠️ Technologies Used

- **Data Collection**: yfinance
- **Data Processing**: pandas, numpy
- **Machine Learning**: scikit-learn, TensorFlow/Keras, Prophet, XGBoost, statsmodels
- **Visualization**: matplotlib, seaborn, plotly
- **Development**: Jupyter Notebook

## 📝 Answers to Common Questions

**Q: How accurate are the predictions?**
- All models include performance metrics (RMSE, MAE, MAPE, R²)
- Confidence intervals show uncertainty ranges
- Best model selected based on quantitative comparison

**Q: Can I use this for actual trading?**
- This is for educational and research purposes only
- Not financial advice
- Always consult with financial professionals

**Q: How to update the data?**
- Re-run the notebook to fetch latest data
- Models will automatically retrain
- Forecasts will update accordingly

**Q: What if I get errors?**
- Ensure all dependencies are installed
- Check Python version (3.8+)
- Verify internet connection for data fetching

## 🔄 Reproducing Results

1. Set up virtual environment: `setup_env.bat`
2. Generate notebook: `python create_notebook.py`
3. Run all cells in `silver_price_analysis.ipynb`
4. Results will be saved to CSV files

## ⚠️ Disclaimer

This analysis is for educational and informational purposes only. It should not be considered as financial advice. Silver prices are subject to various factors including market conditions, economic indicators, and geopolitical events. Always conduct your own research and consult with qualified financial advisors before making investment decisions.

## 📄 License

This project is open source and available under the MIT License.

## 👤 Author

**Business & Economy Analyst**
- Project Focus: Time Series Forecasting & Financial Analysis
- Date: January 2026

## 🙏 Acknowledgments

- Yahoo Finance for providing historical data
- Open source community for amazing ML libraries
- Kaggle community for inspiration and learning

---

**If you found this project helpful, please consider giving it a star ⭐ on GitHub or an upvote on Kaggle!**

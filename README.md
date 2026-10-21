# Capstone-covid-19-forecasting-analysis

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/yogeshkbahl/Capstone-covid-19-forecasting-analysis/blob/main/Capstone_Project_%28Covid_19%29.ipynb)

▶️ **Run it in Google Colab:** click the badge above, then **Runtime → Run all**. The data loads straight from this repo, so no upload is needed.

A comprehensive COVID-19 data analysis and forecasting project using Python, Plotly, and Facebook Prophet. Analyzes global infection trends, calculates recovery and mortality rates, and generates 7-day case predictions using time-series forecasting.

# COVID-19 Forecasting & Analysis

A data-driven analysis of worldwide COVID-19 trends with interactive visualizations and machine learning-based forecasting using Facebook Prophet.

## 📋 Project Overview

This capstone project analyzes global COVID-19 data to identify infection patterns, recovery trends, and mortality rates. Using advanced time-series forecasting techniques, it predicts confirmed case trends for the next 7 days with confidence intervals.

**Key Focus Areas:**
- Global COVID-19 trend analysis over time
- Daily new cases, deaths, and recoveries calculation
- Infection rate and recovery rate analysis
- Interactive data visualization
- 7-day case forecasting using Facebook Prophet

## ✨ Features

- **Data Preprocessing**: Clean, aggregate, and prepare COVID-19 data for analysis
- **Global Trend Analysis**: Visualize confirmed cases, deaths, recovered cases, and active cases over time
- **Daily Metrics Calculation**: Compute daily new cases, deaths, and recoveries with rate of change
- **Rate Analysis**: Calculate infection rates and recovery rates to understand pandemic dynamics
- **Interactive Visualizations**: Dynamic, zoomable Plotly charts for exploring data patterns
- **Time-Series Forecasting**: Facebook Prophet model for 7-day case predictions
- **Confidence Intervals**: Display prediction uncertainty with upper and lower bounds
- **Seasonal Decomposition**: Analyze temporal components of COVID-19 trends

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| **Language** | Python 3 |
| **Data Processing** | Pandas, NumPy |
| **Visualization** | Plotly, Matplotlib |
| **Forecasting** | Facebook Prophet |
| **Notebooks** | Jupyter Notebook / Google Colab |

## 📦 Installation

### Prerequisites
- Python 3.7+
- pip or conda

### Setup

1. **Clone the repository:**
```bash
   git clone https://github.com/yogeshkbahl/Capstone-covid-19-forecasting-analysis.git
   cd Capstone-covid-19-forecasting-analysis
```

2. **Install dependencies:**
```bash
   pip install pandas numpy matplotlib plotly prophet
```

   Or using conda:
```bash
   conda install pandas numpy matplotlib plotly -c conda-forge
   conda install -c conda-forge prophet
```

3. **Dataset:**
   `covid_19_clean_complete.csv` loads automatically from this GitHub repo (no download needed).

## 🚀 Usage

### Running the Analysis

**Option 1: Jupyter Notebook (Recommended)**
```bash
jupyter notebook "Capstone_Project_(Covid_19).ipynb"
```

**Option 2: Google Colab**
1. Click the **Open in Colab** badge at the top of this README
2. Choose **Runtime → Run all**
3. All visualizations will display inline

### Workflow

The notebook executes the following steps:

1. **Install & Import Libraries** - Load required packages
2. **Load Dataset** - Read COVID-19 data from CSV
3. **Data Overview** - Inspect data structure and missing values
4. **Date Conversion** - Format date column as datetime
5. **Global Aggregation** - Sum confirmed cases, deaths, recovered, and active by date
6. **Trend Visualization** - Plot global COVID-19 metrics over time
7. **Daily Metrics** - Calculate daily new cases, deaths, and recoveries
8. **Rate Analysis** - Compute infection and recovery rates
9. **Prophet Preparation** - Format data for forecasting model
10. **Model Training** - Train Facebook Prophet on historical data
11. **Predictions** - Generate 7-day forecasts with confidence bounds
12. **Forecast Visualization** - Plot predictions and seasonal components

## 📊 Example Output

### Global Trends Chart
Displays four time-series lines:
- **Confirmed Cases** (blue): Cumulative confirmed COVID-19 cases
- **Deaths** (red): Cumulative deaths
- **Recovered** (green): Cumulative recoveries
- **Active** (yellow): Currently active cases

### Daily New Cases
Bar/line chart showing new cases reported each day, allowing identification of wave patterns.

### Rate Analysis
Compares infection rate (% change in daily cases) vs. recovery rate over time.

### 7-Day Forecast
Prophet's output includes:
- **Predicted confirmed cases** (yhat): Point estimate for future cases
- **Confidence intervals** (yhat_lower, yhat_upper): Range of prediction uncertainty
- **Trend component**: Overall direction (increasing/decreasing)
- **Seasonal patterns**: Weekly/monthly patterns in case reporting

## 📁 File Structure


## 📈 Dataset Information

**File:** `covid_19_clean_complete.csv`

**Rows:** 49,068 daily records  
**Columns:** 10 fields

| Column | Type | Description |
|--------|------|-------------|
| Province/State | String | Region within country |
| Country/Region | String | Country name |
| Lat | Float | Latitude coordinate |
| Long | Float | Longitude coordinate |
| Date | String | Date of record (YYYY-MM-DD) |
| Confirmed | Integer | Cumulative confirmed cases |
| Deaths | Integer | Cumulative deaths |
| Recovered | Integer | Cumulative recovered cases |
| Active | Integer | Currently active cases |
| WHO Region | String | WHO geographical region classification |

## 🔍 Key Insights Generated

1. **Temporal Trends**: Identify waves and peaks in case progression
2. **Daily Volatility**: Detect spikes in new case reporting
3. **Recovery Patterns**: Understand lag between confirmed cases and recoveries
4. **Mortality Rates**: Track death rate changes over pandemic timeline
5. **Future Outlook**: 7-day predictions for case trend direction

## 🚦 Model Performance Considerations

- **Prophet Strengths**: Handles seasonality, trend changes, and holidays well
- **Forecast Accuracy**: Most reliable for short-term (7-day) predictions
- **Limitations**: Assumes historical patterns continue; may not capture sudden policy changes or variant impacts
- **Uncertainty**: Prediction intervals widen for longer forecast horizons

## 📝 Future Improvements

- Extend forecasts to 14-30 day periods with ensemble methods
- Add regional/country-specific forecasting models
- Incorporate external factors (vaccination rates, policy changes)
- Implement ARIMA or LSTM models for comparison
- Add death and recovery predictions alongside case forecasts
- Develop interactive dashboard for real-time updates
- Integrate live data feeds for continuous model updates
- Add anomaly detection for outbreak identification

## 📄 License

This project is licensed under the MIT License. See the LICENSE file for details.

## 👤 Author

**Yogesh Bahl**

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report issues
- Suggest improvements
- Submit pull requests for new features

This analysis is for educational purposes. Predictions should not be used as the sole basis for critical decision-making. Always consult official health authorities for current COVID-19 information.

---

**Last Updated:** Feb 2026  

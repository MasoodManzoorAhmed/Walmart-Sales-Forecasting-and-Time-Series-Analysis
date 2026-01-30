![Python](https://img.shields.io/badge/Python-3.10-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557C)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-4EABE5)
![Statistics](https://img.shields.io/badge/Statistics-EDA%20%26%20Analysis-brightgreen)
![Time Series](https://img.shields.io/badge/Time%20Series-Forecasting-orange)
![Holt-Winters](https://img.shields.io/badge/Holt--Winters-Exponential%20Smoothing-red)
![Statsmodels](https://img.shields.io/badge/Statsmodels-Time%20Series-purple)
![Retail Analytics](https://img.shields.io/badge/Retail-Analytics-yellowgreen)
![Demand Forecasting](https://img.shields.io/badge/Demand-Forecasting-yellow)
![Seasonality](https://img.shields.io/badge/Seasonality-Holiday%20Impact-blueviolet)
![Data Science](https://img.shields.io/badge/Data%20Science-End--to--End-success)
![Google Colab](https://img.shields.io/badge/Google-Colab-F9AB00)

# Walmart Sales Forecasting & Time Series Analysis

## Project Overview

This project analyzes historical Walmart weekly sales data to understand sales patterns, seasonality, and the impact of holidays. The objective is to build an end-to-end data science workflow that includes exploratory data analysis, statistical insights, and time series forecasting to predict sales for the next 12 weeks.

The project demonstrates how time series forecasting techniques can be applied in a real-world retail business context to support demand planning and operational decision-making.

---

## Dataset Description

- **Dataset:** Walmart Weekly Sales Data  
- **Time Period:** February 2010 – October 2012  
- **Total Records:** 6,435  
- **Total Stores:** 45  

### Features
- `Store` – Store identifier  
- `Date` – Week ending date  
- `Weekly_Sales` – Weekly sales amount  
- `Holiday_Flag` – Holiday indicator  
- `Temperature` – Average weekly temperature  
- `Fuel_Price` – Fuel price  
- `CPI` – Consumer Price Index  
- `Unemployment` – Unemployment rate  

---

## Tools & Technologies Used

- **Programming Language:** Python  
- **Data Analysis:** Pandas, NumPy  
- **Visualization:** Matplotlib, Seaborn  
- **Statistics & EDA:** Descriptive statistics, correlation analysis  
- **Time Series Forecasting:** Statsmodels  
- **Model Used:** Holt-Winters Exponential Smoothing  
- **Environment:** Google Colab / Jupyter Notebook  

---

## Exploratory Data Analysis (EDA)

The dataset was explored to understand its structure, quality, and underlying patterns.

### EDA Steps Performed
- Checked data types and missing values  
- Converted date column to datetime format  
- Generated statistical summaries for numerical features  
- Visualized sales distribution using histograms and boxplots  
- Identified valid high-value outliers  

### Key EDA Insights
- No missing values were found in the dataset  
- Weekly sales distribution is right-skewed  
- High sales outliers are associated with holidays and large stores  
- Outliers were retained as they represent genuine business events  

---

## Holiday Impact Analysis

Average weekly sales were compared between holiday and non-holiday weeks.

- **Non-holiday average sales:** ~1.04 million  
- **Holiday average sales:** ~1.12 million  

Holiday weeks show approximately **8% higher sales**, confirming the strong impact of holidays on retail demand.

---

## Correlation Analysis

Correlation analysis was conducted between weekly sales and external variables such as temperature, fuel price, CPI, and unemployment.

### Findings
- Weekly sales have weak correlation with macroeconomic variables  
- Slight negative correlation with unemployment and CPI  
- Sales are primarily driven by seasonal and store-level factors  

---

## Time Series Analysis

Store-level time series plots revealed clear seasonal patterns in weekly sales, with recurring peaks during holiday periods. This confirmed the suitability of seasonal time series models for forecasting.

---

## Sales Forecasting

Holt-Winters Exponential Smoothing was applied to model trend and seasonality in weekly sales data.

### Forecasting Approach
- Built individual models for each of the 45 stores  
- Used a seasonal period of 52 weeks  
- Generated **12-week sales forecasts for all stores**  

The forecasts indicate increased sales during upcoming holiday periods and provide valuable insights for short-term planning.

---

## Results & Business Impact

- Successfully generated store-wise 12-week sales forecasts  
- Identified strong seasonality and holiday-driven demand  
- Insights support:
  - Inventory optimization  
  - Workforce planning  
  - Promotion scheduling  

---

## Conclusion

This project demonstrates a complete end-to-end data science workflow for retail sales forecasting. The Holt-Winters model effectively captured seasonal patterns and trends in Walmart sales data, making it a reliable approach for short-term demand forecasting.

The results can help retail businesses make data-driven decisions to improve operational efficiency and customer satisfaction.

---

## Future Enhancements

- Perform backtesting to evaluate forecast accuracy  
- Compare Holt-Winters with ARIMA or machine learning models  
- Incorporate promotional and regional factors  
- Build an interactive dashboard for real-time forecasting  

---

## Author

**Masood Manzoor Ahmed**  
Data Science & Machine Learning Enthusiast

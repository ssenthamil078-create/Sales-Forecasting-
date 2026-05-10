# Sales Forecasting Using Time Series Analysis

## Project Overview

This project focuses on forecasting future retail sales using historical weekly sales data. The analysis identifies trends, seasonal patterns, holiday effects, store-level performance, department-level contribution, and promotional impact.

The goal is to predict future sales and compare forecasted values with actual sales trends using a classical time-series decomposition approach.

## Objective

- Analyze historical retail sales data
- Identify seasonal and trend-based sales patterns
- Forecast future weekly sales
- Study the impact of holidays and markdown promotions
- Compare store type and department-level performance
- Visualize actual sales vs forecasted sales

## Dataset

The project uses four sales-related files:

- `train.csv`
- `features.csv`
- `stores.csv`
- `test.csv`

These files contain weekly sales, store details, markdown promotions, holiday indicators, and external economic features.

## Methodology

Since Prophet and statsmodels were not available in the working environment, the forecasting model uses a classical seasonal decomposition method.

### Model Used

Seasonal Decomposition STL-style approach:

- 4-week rolling trend calculation
- 52-week seasonal pattern extraction
- Linear trend extrapolation
- Weekly retail sales forecasting

This approach captures the core time-series behavior similar to ARIMA and Prophet for weekly sales data.

## Key Insights

- Average weekly sales are around `$47M`
- Sales trend is broadly flat with a slight upward movement from 2010 to 2012
- Seasonality is the strongest driver of sales
- Christmas week reaches around `$81M`, almost double a typical January week
- Thanksgiving creates a secondary sales spike of around `$65M`
- Holiday impact is concentrated mainly around Thanksgiving and Christmas
- Holiday flag weeks show an average lift of about `7.1%`
- Forecast from November 2012 to January 2013 predicts:
  - Thanksgiving spike around `$61.5M`
  - Christmas peak around `$66.8M`
  - Post-holiday sales dip in early January
- Store Type A contributes around `60%` of total revenue
- Store Type B contributes around `30%`
- Store Type C contributes around `10%`
- Top departments by revenue:
  - Department 92: `$484M`
  - Department 95: `$449M`
  - Department 38: `$393M`
- Markdown promotions have weak correlation with sales, ranging from `0.02` to `0.09`

## Tools and Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Time Series Analysis

## Project Workflow

1. Import sales datasets
2. Clean and preprocess data
3. Merge train, features, and stores data
4. Convert date column into datetime format
5. Perform exploratory data analysis
6. Analyze weekly sales trend
7. Study holiday and seasonal impact
8. Analyze store type performance
9. Analyze department-level sales contribution
10. Apply seasonal decomposition forecasting
11. Forecast future sales
12. Visualize actual vs forecasted sales

## Visualizations Included

- Weekly sales trend
- Holiday vs non-holiday sales comparison
- Store type revenue contribution
- Top department sales performance
- Actual vs forecasted sales
- Seasonal sales patterns
- Markdown correlation analysis
<img width="1892" height="735" alt="Screenshot 2026-05-10 222953" src="https://github.com/user-attachments/assets/d55586fd-2c71-443e-a811-02b990cf5cd8" />
<img width="1881" height="421" alt="Screenshot 2026-05-10 223022" src="https://github.com/user-attachments/assets/7f42db1d-3b56-43a9-a2d2-311f02760f51" />
<img width="1883" height="406" alt="Screenshot 2026-05-10 223011" src="https://github.com/user-attachments/assets/02765cfa-d0bb-47c2-b3a5-a57683b93aef" />

## Forecasting Result

The model successfully captures major seasonal spikes during Thanksgiving and Christmas. It shows that retail sales are strongly seasonal, with holiday periods contributing significantly to revenue peaks.

## Conclusion

This project shows that sales forecasting is highly useful for retail businesses to plan inventory, staffing, and promotional strategies. The analysis proves that seasonality and store size have a stronger impact on sales than markdown discounts.

## Future Improvements

- Apply ARIMA and SARIMA models
- Use Facebook Prophet for advanced forecasting
- Build LSTM deep learning model
- Deploy forecasting dashboard using Streamlit
- Connect Power BI dashboard for business reporting
- Add real-time sales prediction system

## Author

**Sendhamil Selvan**  
Artificial Intelligence and Data Science Student  
Interested in Data Analytics, Cloud Computing, and AI Projects


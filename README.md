# Household Power Consumption Analysis: Time Series Forecasting, Fourier Transform, Multiple Linear Regression & Hypothesis Testing
----
The objective of this project is to recognize patterns and trends in household energy usage by
examining historical power consumption data, improve energy management with predictive
insights, and detect irregularities in consumption behavior. It will assess
how voltage and current levels affect power usage, offering practical suggestions to improve
energy efficiency and optimize grid operation.

This project performs a comprehensive analysis of household power consumption using several advanced data science techniques:
- **Time Series Forecasting:** To predict future consumption trends and identify seasonal patterns.
- **Fourier Transform:** To decompose the power consumption signal into its frequency components, revealing dominant cycles.
- **Multiple Linear Regression (MLR):** To model the relationship between independent factors (such as weather conditions and time variables) and power consumption.
- **Hypothesis Testing:** To statistically validate observed trends and patterns.
-----

## Key Components

### Data Preprocessing
- Cleans and prepares the dataset.
- Handles missing values and performs feature engineering to enhance the analysis.

### Time Series Forecasting
- Models the temporal dynamics of power consumption.
- Identifies seasonal trends and long-term behavior for robust forecasting.

### Fourier Transform Analysis
- Converts the time series into the frequency domain.
- Highlights dominant periodic signals, such as daily and weekly consumption cycles.

### Multiple Linear Regression
- Develops predictive models to quantify the impact of various factors on power consumption.
- Identifies significant predictors influencing energy usage.

### Hypothesis Testing
- Uses statistical tests (e.g., t-tests, ANOVA) to confirm the significance of observed trends.
- Validates the model outcomes and data-driven insights.

  
## Data Overview
- **Source:** UCI Machine Learning Repository
- **Period:** December 2006 to November 2010
- **Data Points:** Over 2 million records from a single household
- **Key Features:**
  - *Global_active_power*: Overall household power consumption
  - *Global_reactive_power*: Reactive power usage
  - *Voltage*: Voltage level
  - *Global_intensity*: Current intensity
  - *Sub-metering*: Device-level power usage

---

## Methodology

### Time Series Forecasting
- **Model:** SARIMAX (Seasonal ARIMA with exogenous variables)
- **Approach:**
  - Data preprocessing: Sampling to monthly aggregates
  - Seasonality and stationarity checks
  - Model parameter selection via auto-arima search
  - Training and validation to forecast the next 24 months


### Fourier Transform Analysis
- **Purpose:**  
  Convert time-domain data to the frequency domain to uncover hidden periodic patterns.
- **Outcome:**  
  Identification of dominant frequencies (annual and semi-annual cycles) that drive energy consumption.

### Multiple Linear Regression (MLR)
- **Data Preparation:**  
  Interpolated null values, engineered time-based features (hour, day of week), and standardized predictors.
- **Predictors:**  
  Global_reactive_power, Voltage, Sub_metering values, Hour, Day_of_Week
- **Target:**  
  Global_active_power
- **Results:**
  - Standard Linear Regression
  - Ridge & SGD Regression: Similar performance to linear regression
  - ElasticNet Regression: Underperformed 
- **Insights:**  
  Linear models capture significant variance in power consumption, although additional tuning and data transformation may improve robustness.

### Hypothesis Testing
- **Objective:**  
  To test if power consumption differs significantly between weekdays and weekends.
- **Method:**  
  Independent t-test
- **Findings:**  
  The null hypothesis was rejected, confirming that average Global Active Power is higher on weekends.

---
## Analysis & Findings
- **Time Series Analysis:**  
  Forecasting models captured both seasonal and trend components, leading to accurate predictions of future consumption.
  
- **Frequency Analysis:**  
  Fourier transform analysis revealed strong periodicities, consistent with expected daily and weekly cycles.
  
- **Regression Modeling:**  
  The MLR approach identified key factors that significantly affect power consumption, offering actionable insights.
  
- **Statistical Validation:**  
  Hypothesis tests confirmed that the observed differences and trends are statistically significant, supporting the robustness of the findings.
---

## Business Insights & Recommendations

### Demand Forecasting & Consumer Analytics
- **Accurate Demand Forecasting:**  
  Time series models (SARIMAX) enable energy providers to predict consumption trends, ensuring better grid stability and infrastructure planning.
- **Consumer Behavior Analysis:**  
  Fourier Transform reveals periodic patterns that can be used to understand and segment consumer usage, leading to more tailored energy conservation initiatives.

### Optimizing Energy Pricing
- **Dynamic Pricing Strategies:**  
  - Adjust pricing based on demand forecasts; charge premium rates during peak usage periods (e.g., weekends) and offer discounts during off-peak times.
  - Utilize regression insights to fine-tune price adjustments that reflect real consumption drivers.
- **Targeted Offers:**  
  Develop promotions based on detailed consumer analytics, such as time-of-day usage, to incentivize energy savings and reduce grid stress.

### Future Enhancements
- **Model Refinements:**  
  Explore intraday consumption patterns and incorporate external factors (weather, economic indicators) to enhance forecasting accuracy.
- **Extended Hypotheses:**  
  Investigate other consumption aspects such as peak versus non-peak usage to further optimize pricing and demand management.

Overall, we analyzed key metrics like Global Active/Reactive Power, Voltage, Global Intensity, and Sub-metering values. Using Multiple Linear Regression, and predicted consumption trends, employed Time Series Forecasting visualizations for pattern analysis, applied Fourier Transform to extract frequency components, and conducted Statistical Hypothesis Testing to validate insights. This project gave us insights into which months power consumption of appliances in household spikes which would be beneficial for demand/resource planning, optimizing pricing strategies and and energy efficiency. 


## How to Run
1. Open the relevant Jupyter Notebooks in your preferred environment (e.g., [Google Colab](https://colab.research.google.com)).
2. Ensure the dataset is accessible in the specified path.
3. Execute the notebooks in sequence to carry out data preprocessing, analysis, and model evaluation.
4. Review the output visuals and statistical summaries to understand the household power consumption behavior.


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

## Analysis & Findings
- **Time Series Analysis:**  
  Forecasting models captured both seasonal and trend components, leading to accurate predictions of future consumption.
  
- **Frequency Analysis:**  
  Fourier transform analysis revealed strong periodicities, consistent with expected daily and weekly cycles.
  
- **Regression Modeling:**  
  The MLR approach identified key factors that significantly affect power consumption, offering actionable insights.
  
- **Statistical Validation:**  
  Hypothesis tests confirmed that the observed differences and trends are statistically significant, supporting the robustness of the findings.

## How to Run
1. Open the relevant Jupyter Notebooks in your preferred environment (e.g., [Google Colab](https://colab.research.google.com)).
2. Ensure the dataset is accessible in the specified path.
3. Execute the notebooks in sequence to carry out data preprocessing, analysis, and model evaluation.
4. Review the output visuals and statistical summaries to understand the household power consumption behavior.


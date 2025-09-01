# SAF Adoption and Fuel Consumption Prediction and Analysis

This project provides an in-depth analysis and prediction of aviation fuel consumption, with a focus on the potential impact of Sustainable Aviation Fuel (SAF) adoption. The analysis is conducted using a Jupyter Notebook and various Python libraries for data manipulation, time series forecasting, and visualization.

## Project Description

The aviation industry is a significant contributor to global CO2 emissions. Sustainable Aviation Fuel (SAF) presents a promising solution to mitigate this impact, with the potential to reduce lifecycle carbon emissions by up to 80%. This project explores future aviation fuel consumption trends and models the effects of different SAF adoption scenarios.

The analysis utilizes a publicly available dataset on air transport CO2 emissions and employs three different forecasting models:
*   **Linear Regression**
*   **SARIMAX (Seasonal Auto-Regressive Integrated Moving Average with eXogenous factors)**
*   **LSTM (Long Short-Term Memory)**

After evaluating the models, the most accurate one is used to forecast emissions up to 2050. These forecasts are then used as a baseline to analyze the potential emissions reductions under various SAF adoption scenarios, including those recommended by the ICAO and different policy frameworks.

## Getting Started

### Prerequisites

*   Python 3.x
*   Jupyter Notebook
*   The following Python libraries:
    *   pandas
    *   numpy
    *   matplotlib
    *   seaborn
    *   scikit-learn
    *   statsmodels
    *   tensorflow
    *   pmdarima

You can install the required libraries using pip:
`pip install pandas numpy matplotlib seaborn scikit-learn statsmodels tensorflow pmdarima`

### Running the Notebook

1.  Clone this repository to your local machine.
2.  Navigate to the project directory.
3.  Launch Jupyter Notebook:
    `jupyter notebook`
4.  Open the `SAF Adaption and Fuel Consmption Prediction and Analysis.ipynb` file.
5.  Run the cells sequentially to reproduce the analysis.

## Notebook Structure and Methodology

The Jupyter Notebook is organized into the following sections:

1.  **Data Loading and Preprocessing:**
    *   The CO2 emissions dataset is loaded.
    *   The data is filtered to focus on monthly CO2 emissions.

2.  **Exploratory Data Analysis (EDA):**
    *   The time series data is plotted to visualize trends and seasonality.
    *   Seasonal decomposition is performed to separate the trend, seasonal, and residual components of the time series.
    *   The Augmented Dickey-Fuller (ADF) test is used to check for the stationarity of the time series.

3.  **Time Series Forecasting:**
    *   **Model Training:** Linear Regression, SARIMAX, and LSTM models are trained on the historical emissions data.
    *   **Model Evaluation:** The models are evaluated using MAE, RMSE, and R-squared metrics to select the best-performing model.
    *   **Forecasting:** The SARIMAX model is used to forecast CO2 emissions up to 2050.

4.  **SAF Adoption Scenario Analysis:**
    *   Different scenarios for SAF adoption are defined based on ICAO recommendations, policy frameworks (mandatory, subsidy-based, no incentive), and varying levels of adoption rates.
    *   The impact of these scenarios on the forecasted emissions is calculated and visualized.

## Results

The analysis provides a forecast of aviation CO2 emissions up to 2050 and demonstrates the significant potential for emissions reduction through the adoption of SAF. The different scenarios highlight the importance of policy incentives and ambitious adoption targets in achieving a more sustainable aviation future.

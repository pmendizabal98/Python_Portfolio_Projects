The aim of this project is to conduct a correlation analysis between weather data and solar panel energy generation in a place located in the UK. Additionally, a machine learning prediction model will be developed using a 14-day weather forecast to estimate the solar panel generation in the community center.

This repository includes three Jupyter notebooks that perform data analytics and predictions on weather data and solar panel power generation in the community center. The notebooks make use of a public API to retrieve weather data and forecast information for analysis.

# Weather_solar_energy_correlation_analysis.ipynb

This notebook is the overall project with the Correlation Analysis and the machine learning model (3 machine learning model tested) to make predictions over the 4 best correlated weather variables that affect the solar panel generations.

The steps in this notebook include:

- A check for multicollinearity is conducted to identify potential issues caused by high correlations between predictor variables. (Given that in the past notebook, we saw that 4 weather variables has some correlation with the solar panel generation)
- PCA is applied to address multicollinearity issues by transforming correlated variables into a new set of uncorrelated variables called principal components. 
- A multiple linear regression model is built using the transformed principal components as predictors
- The goodness of fit of the linear regression model is assessed using the R-squared value, which measures the proportion of variance in solar power generation explained by the predictors
- Cross-validation is performed to evaluate the model's performance and generalization ability.

# Historic_weather_and_solar_gen_correlation.ipynb

In this notebook, weather data is retrieved from a public API and cleaned for further analysis. The steps involved in this notebook are as follows:

- Retrieving weather data using a public API.
- Cleaning the weather data to remove any inconsistencies or missing values.
- Extracting power generation data from the solar panel in the community centre.
- Analyzing the relationship between weather data and power generation.
- Finding correlations between weather variables and power generation.

# 14_day_weather_Forecast.ipynb

The second notebook focuses on retrieving forecast weather data from the same public API for further analysis. The steps in this notebook include:

- Retrieving forecast weather data using the public API.
- Performing analysis on the forecasted weather data.
- Exploring any patterns or trends in the forecasted weather.
- Analyzing how forecasted weather may impact power generation from the solar panel.

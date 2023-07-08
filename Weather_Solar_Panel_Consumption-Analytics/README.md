This repository contains two Jupyter notebooks that perform data analytics on weather data and power generation from a solar panel in a community centre in the UK. The notebooks utilize a public API to retrieve weather data and forecast information for analysis.
Historic_weather_and_solar_gen_correlation

# Historic_weather_and_solar_gen_correlation

In this notebook, weather data is retrieved from a public API and cleaned for further analysis. The steps involved in this notebook are as follows:

- Retrieving weather data using a public API.
- Cleaning the weather data to remove any inconsistencies or missing values.
- Extracting power generation data from the solar panel in the community centre.
- Analyzing the relationship between weather data and power generation.
- Finding correlations between weather variables and power generation.

# 14_day_weather_Forecast

The second notebook focuses on retrieving forecast weather data from the same public API for further analysis. The steps in this notebook include:

- Retrieving forecast weather data using the public API.
- Performing analysis on the forecasted weather data.
- Exploring any patterns or trends in the forecasted weather.
- Analyzing how forecasted weather may impact power generation from the solar panel.

# Solar_Energy_Prediction_Weather_data

In this notebook, a machine learning model (multiple linear regression) was used to make predictions over the 4 best correlated weather variables that affect the solar panel generations.
The steps in this notebook include:

- A check for multicollinearity is conducted to identify potential issues caused by high correlations between predictor variables. (Given that in the past notebook, we saw that 4 weather variables has some correlation with the solar panel generation)
- PCA is applied to address multicollinearity issues by transforming correlated variables into a new set of uncorrelated variables called principal components. 
- A multiple linear regression model is built using the transformed principal components as predictors
- The goodness of fit of the linear regression model is assessed using the R-squared value, which measures the proportion of variance in solar power generation explained by the predictors
- Cross-validation is performed to evaluate the model's performance and generalization ability.

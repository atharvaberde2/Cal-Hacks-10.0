# Introduction
Imagine meticulously planning a fantastic vacation months in advance, only to have it ruined by unexpected rain, or extreme weather.
This frustration, coupled with the noticeable effects of global warming in our hometown of San Jose, led my friend and I to create a weather prediction model to ensure that people can make informed decisions based on accurate forecasts.

# How we built it
We first extracted data from National Weather Service and used Pandas to create a Data Table. There were three target variables: Min Temperature, Max Temperature, Precipitation amount. We ran a RandomForestRegressor along with Hyperparameter Tuning to predict Precipitation amount, achieving a Mean Absolute Error of 0.01. To predict Min temperature, we used a pipeline of Polynomial features and Ridge Regression, and we acieved an 87% accuracy. We used two different models to predict Max Temperature, VotingRegressor and Gradient Boositng Regressor, achieving accuracy of 91% and 92% respectively. 

# Challenges we ran into
Initially, we used linear regression to predict all three target variables, but the accuracy score was very low because our data had a convex shape. Recognizing this limitation, we experimented with different models for each target variable and utilized Hyperparameter Tuning, which led to significantly improved accuracy. Collaborating with my friend, we divided tasks and tackled these challenges together, which deepened our understanding of machine learning algorithms.

# Introduction
Imagine meticulously planning a fantastic vacation months in advance, only to have it ruined by unexpected rain, or extreme weather.
This frustration, coupled with the noticeable effects of global warming in our hometown of San Jose, led my friend and I to create a weather prediction model to ensure that people can make informed decisions based on accurate forecasts.

# How we built it
We first extracted data from National Weather Service and used Pandas to create a Data Table. There were three target variables: Min Temperature, Max Temperature, Precipitation amount. We experimented with several models, including logistic regression, support vector machines, and neural networks, to predict precipitation and minimum/maximum temperatures. We found that a RandomForestRegressor would best predict the amount of precipitation, achieving a Mean Absolute Error of 0.01. To predict the minimum temperature, we found that a pipeline of Polynomial Features and Ridge Regression would yield the best performance, achieving an $\boldsymbol {R^2}$ of 87%. For maximum temperature, we found that a Gradient Boosting Regressor provided the optimal performance, posting an $\boldsymbol {R^2}$ of 91%.

# Challenges we ran into
Initially, we used linear regression to predict all three target variables, but the accuracy score was very low because our data had a convex shape. Recognizing this limitation, we experimented with different models for each target variable and utilized Hyperparameter Tuning, which led to significantly improved accuracy. Collaborating with my friend, we divided tasks and tackled these challenges together, which deepened our understanding of machine learning algorithms.

# Results and Impact
Our model’s accurate predictions can help farmers plan their activities better, travelers make informed decisions, and even local businesses optimize their operations. Companies can adjust their supply chain logistics through our model, minimizing disruptions caused by adverse weather conditions. Retail businesses can adjust inventory and staffing levels based on expected weather conditions, enhancing operational efficiency and improving customer satisfaction.

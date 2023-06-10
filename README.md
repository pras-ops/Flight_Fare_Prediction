# Flight Fare Prediction using ML and Auto SK Learn (Auto ML)

This project focuses on predicting the fare of a flight based on input data using traditional machine learning techniques and Auto SK Learn, which is an Auto ML library.

## Context

Flight ticket prices are often unpredictable and can vary significantly from day to day. This project aims to create a machine learning model that can predict flight prices based on various attributes. The dataset used includes flight ticket prices for different airlines between the months of March and June 2019, as well as information about the source, destination, route, departure time, arrival time, duration, and additional details of the flights.

## Notebook Sections

The notebook includes the following sections:

1.  Data Analysis: This section analyzes the dataset, exploring relationships between different variables and the fare prices. It includes visualizations and insights on airlines, sources, destinations, and duration.
    
2.  Feature Engineering: In this section, feature engineering techniques are applied to preprocess the data and extract useful information. Date of journey is split into separate day, month, and year columns. Additional information, arrival time, and total stops are processed and converted to numerical values.
    
3.  Feature Selection: This section covers feature selection using Lasso regression and ExtraTreesRegressor to identify the most important features for the model.
    
4.  Model Building using ML: The dataset is split into training and testing sets, and a RandomForestRegressor model is built using the selected features. The model's performance is evaluated using metrics such as mean absolute error (MAE), mean squared error (MSE), root mean squared error (RMSE), and R-squared.
    
5.  Hyperparameter Tuning: The RandomizedSearchCV technique is used to find the optimal hyperparameters for the RandomForestRegressor model.
    
6.  Model Building using Auto SK Learn (Auto ML): This section demonstrates the use of Auto SK Learn, an automated machine learning library. The AutoSklearnRegressor is trained on the same training data, and its performance is evaluated using the same metrics as the previous model.
    

## Report

The findings of the project include:

-   The analysis revealed that Jet Airways Business has the highest fare among the airlines.
![download](https://github.com/pras-ops/Flight_Fare_Prediction/assets/56476064/3a71a6fd-cf17-43d2-a0b9-da2a592e6d7b)
-   The source and destination cities also have a significant impact on flight prices.
![download](https://github.com/pras-ops/Flight_Fare_Prediction/assets/56476064/9372e8c7-de91-4c51-92c2-ccbc321c1cf3)
-   Feature engineering techniques, such as splitting date of journey and converting categorical variables, were applied to preprocess the data.
-   Feature selection helped identify the most important features for the models.
-   The RandomForestRegressor model achieved a good performance with reasonable MAE, MSE, RMSE, and R-squared values.
-   Hyperparameter tuning further improved the performance of the RandomForestRegressor model.
-   Auto SK Learn (Auto ML) using the AutoSklearnRegressor also provided competitive results, automatically selecting and optimizing the model.

These findings demonstrate the effectiveness of machine learning techniques in predicting flight fares and highlight the potential of Auto ML libraries for automating the model selection and optimization process.

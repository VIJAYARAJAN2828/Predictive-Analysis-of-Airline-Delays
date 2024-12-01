Predicting Flight Delays Using Machine Learning

Project Overview :

This project focuses on analyzing the on-time performance of domestic flights in the United States, using data provided by the U.S. Department of Transportation's Bureau of Transportation Statistics (BTS). The dataset comprises 1,247,488 rows and 30 columns, offering a comprehensive overview of flight schedules, delays, cancellations, diversions, and their causes.
The primary goal is to identify key factors affecting air travel punctuality and develop predictive models to anticipate flight delays. This analysis aims to provide actionable insights for airlines, passengers, and policymakers.

Dataset :

The dataset includes detailed attributes such as:Flight Information: Year, Month, DayofMonth, DayOfWeek, UniqueCarrier, FlightNum, TailNum
Schedule and Timing: DepTime, CRSDepTime, ArrTime, CRSArrTime, ActualElapsedTime, CRSElapsedTime, AirTime
Delays and Causes: ArrDelay, DepDelay, CarrierDelay, WeatherDelay, NASDelay, SecurityDelay, LateAircraftDelay
Flight Status: Cancelled, CancellationCode, Diverted
Other Metrics: Origin, Dest, Distance, TaxiIn, TaxiOut


Problem Statement : The problem statement for this project is: "Identify the key factors influencing air travel punctuality and develop predictive models to mitigate delays."

Methodology
* Exploratory Data Analysis (EDA):
* Distribution and trends in delays.
* Correlation between different delay types and flight features.


Data Preprocessing:

*Handling missing values.
*Encoding categorical variables.
*Feature scaling and selection.
*Model Development: Several machine learning models were trained and evaluated:

Linear Regression
Ridge Regression
Decision Tree Regressor
Random Forest Regressor
Gradient Boosting Regressor
AdaBoost Regressor
Hyperparameter Tuning:

Grid Search and Randomized Search were employed to optimize model performance.

Model Performance : 


| Model                          | RMSE Test | R² Test | MAPE Test |
|--------------------------------|-----------|---------|-----------|
| LinearRegression               | 0.4103    | 0.8307  | 1.0029    |
| Ridge                          | 0.4103    | 0.8307  | 1.0029    |
| DecisionTreeRegressor          | 0.3439    | 0.8810  | 0.8713    |
| AdaBoostRegressor              | 0.7024    | 0.5038  | 2.6344    |
| RandomForestRegressor          | 0.2371    | 0.9435  | 0.6305    |
| RandomForestRegressor (Tuned)  | 0.2398    | 0.9422  | 0.6329    |
| GradientBoostingRegressor      | 0.2864    | 0.9175  | 0.7923    |
| DecisionTreeRegressor (Tuned)  | 0.2763    | 0.9232  | 0.7432    |
| Ridge (Tuned)                  | 0.4103    | 0.8307  | 1.0029    |



Key Insights: Random Forest Regressor (with and without tuning) achieved the best performance, indicating its robustness in handling complex relationships in the data.
Delay-related features, such as DepDelay and ArrDelay, were significant predictors of overall flight performance.
External factors like WeatherDelay also played a critical role in determining flight punctuality.


Conclusion : This project successfully demonstrates the use of machine learning to predict flight delays and highlights the critical factors influencing air travel punctuality. The insights gained can help airlines optimize operations and improve customer experience.

Future Work
Incorporate real-time data to enhance model predictions.
Develop a dashboard for dynamic delay prediction and visualization.
Explore advanced ensemble methods for improved accuracy.

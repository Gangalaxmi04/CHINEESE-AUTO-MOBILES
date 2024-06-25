# Car Price Prediction for Geely Auto
Project Overview
Geely Auto, a Chinese automobile company, plans to enter the US market by setting up a local manufacturing unit. To compete effectively with US and European manufacturers, Geely Auto needs to understand the factors affecting car prices in the American market. This project aims to identify significant variables that predict car prices and evaluate how well these variables describe car prices.

Dataset Description
The dataset contains various features of cars, including technical specifications and pricing, gathered from different market surveys in the American market. The dataset consists of 205 rows and 26 columns, each representing a unique car and its attributes.
Dataset Description
The dataset contains various features of cars, including technical specifications and pricing, gathered from different market surveys in the American market. The dataset consists of 205 rows and 26 columns, each representing a unique car and its attributes.

Features
car_ID: Unique identifier for each car.
symboling: Risk factor assigned to the car (+3 indicates risky, -3 indicates safe).
CarName: The name and model of the car.
fueltype: Fuel type of the car (e.g., gas, diesel).
aspiration: Aspiration type (std, turbo).
doornumber: Number of doors (two, four).
carbody: Body style (convertible, sedan, hatchback, etc.).
drivewheel: Type of drive wheel (fwd, rwd, 4wd).
enginelocation: Location of the engine (front, rear).
wheelbase: Wheelbase measurement.
enginesize: Size of the engine.
fuelsystem: Type of fuel system (e.g., mpfi, idi).
boreratio: Bore ratio of the engine.
stroke: Stroke measurement.
compressionratio: Compression ratio of the engine.
horsepower: Horsepower of the engine.
peakrpm: Peak revolutions per minute (RPM).
citympg: City mileage.
highwaympg: Highway mileage.
price: Price of the car (target variable).
# Data Cleaning and Preprocessing
Removing Duplicates: Removed any duplicate records to ensure data quality.
Label Encoding: Applied label encoding to categorical variables (e.g., fueltype, aspiration, doornumber, carbody, drivewheel, enginelocation, fuelsystem).
Handling Multicollinearity: Removed features that exhibited high multicollinearity to improve model performance and interpretability.
Modeling
Two models were used to predict car prices: Linear Regression and Random Forest Regressor.

# Linear Regression

Achieved an R² score of 77%.
Simpler model with less variance, but potentially higher bias.
# Random Forest Regressor

Achieved an R² score of 90% with 5-fold cross-validation (cv=5).
More complex model with higher variance and lower bias.


Conclusion
The Random Forest Regressor, with an R² score of 90%, proved to be more effective in predicting car prices compared to the Linear Regression model.
Significant variables influencing car prices include enginesize, horsepower, carbody, and drivewheel.

T





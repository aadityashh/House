# House Price Prediction Model 

This project implements a House Price Prediction model using Linear Regression. The model is trained to predict house prices based on various features such as the number of bedrooms, bathrooms, square footage, and other relevant attributes.


## Project Overview

The primary objective of this project is to build a regression model that can accurately predict house prices. The model uses Linear Regression to understand the relationship between house features and their sale prices.


### Dataset
The dataset used for training the model contains various features of houses, including:

- Sale Price
- Number of Bedrooms
- Number of Bathrooms
- Flat Area (in Sqft)
- Lot Area (in Sqft)
- Number of Floors
- Waterfront View
- Condition of the House
- Overall Grade
- Area of the House from Basement (in Sqft)
- Basement Area (in Sqft)
- Age of House (in Years)
- Renovated Year
- Zipcode
- Latitude
- Longitude
- Living Area after Renovation (in Sqft)


### Model

The model uses Linear Regression to predict house prices. Linear Regression is a simple yet powerful algorithm for modeling the linear relationship between dependent and independent variables.


### Features
- Input: The model takes various house attributes as input.
- Output: The model predicts the sale price of the house.


### Usage

```
import pandas as pd

# Example data
data = {
    'No of Bedrooms': 3,
    'No of Bathrooms': 2.25,
    'Flat Area (in Sqft)': 2570.0,
    'Lot Area (in Sqft)': 7242.0,
    'No of Floors': 2.0,
    'Waterfront View': 'No',
    'Condition of the House': 'Fair',
    'Overall Grade': 7,
    'Area of the House from Basement (in Sqft)': 2170.0,
    'Basement Area (in Sqft)': 400,
    'Age of House (in Years)': 67,
    'Renovated Year': 1991,
    'Zipcode': 98125.0,
    'Latitude': 47.7210,
    'Longitude': -122.319,
    'Living Area after Renovation (in Sqft)': 1690.0
}

# Convert the data to a DataFrame and make predictions
df = pd.DataFrame([data])
predicted_price = model.predict(df.drop(columns=['Sale Price']))
print(f"Predicted Sale Price: {predicted_price[0]}")
```

### Evaluation
The model was evaluated using metrics such as Mean Squared Error (MSE) and R-squared (R²). The performance of the model can be further improved by experimenting with feature engineering, hyperparameter tuning, and exploring more advanced models.


### Contributing
If you want to contribute to this project, please fork the repository and submit a pull request.

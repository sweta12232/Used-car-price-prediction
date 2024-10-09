# 🚗 Used Car Price Prediction

This repository contains a machine learning project aimed at predicting the prices of used cars based on various features such as car model, year, mileage, fuel type, and more. The goal is to build an accurate model that can help sellers and buyers estimate the market value of a used car.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Features](#features)
- [Installation](#installation)
- [Modeling Process](#modeling-process)
- [Results](#results)
- [Future Improvements](#future-improvements)
- [Contributing](#contributing)


## Project Overview

This project explores the relationship between a car's attributes and its price to build a predictive model. The objective is to use machine learning techniques to predict the price of a used car based on various factors like the car’s age, mileage, make, fuel type, and more.

## Dataset

The dataset used in this project contains information about used cars, including the following features:

| Unnamed: 0 | Name                             | Location   | Year | Kilometers Driven | Fuel Type | Transmission | Owner Type | Mileage    | Engine | Power    | Seats | Price |
|------------|----------------------------------|------------|------|-------------------|-----------|--------------|------------|------------|--------|----------|-------|-------|
| 0          | Maruti Wagon R LXI CNG           | Mumbai     | 2010 | 72000             | CNG       | Manual       | First      | 26.6 km/kg | 998 CC | 58.16 bhp | 5.0   | 1.75  |
| 1          | Hyundai Creta 1.6 CRDi SX Option | Pune       | 2015 | 41000             | Diesel    | Manual       | First      | 19.67 kmpl | 1582 CC| 126.2 bhp | 5.0   | 12.50 |
| 2          | Honda Jazz V                     | Chennai    | 2011 | 46000             | Petrol    | Manual       | First      | 18.2 kmpl  | 1199 CC| 88.7 bhp  | 5.0   | 4.50  |
| 3          | Maruti Ertiga VDI                | Chennai    | 2012 | 87000             | Diesel    | Manual       | First      | 20.77 kmpl | 1248 CC| 88.76 bhp | 7.0   | 6.00  |
| 4          | Audi A4 New 2.0 TDI Multitronic  | Coimbatore | 2013 | 40670             | Diesel    | Automatic    | Second     | 15.2 kmpl  | 1968 CC| 140.8 bhp | 5.0   | 17.74 |

The dataset includes the following features for each car:
- `Name`: The car's make and model.
- `Location`: City where the car is being sold.
- `Year`: Year of manufacture.
- `Kilometers_Driven`: Total kilometers driven.
- `Fuel_Type`: Type of fuel used (CNG, Diesel, Petrol).
- `Transmission`: Manual or automatic transmission.
- `Owner_Type`: Whether the car is first-hand, second-hand, etc.
- `Mileage`: Mileage in km/kg or kmpl.
- `Engine`: Engine displacement in cubic centimeters (CC).
- `Power`: Power output of the car in brake horsepower (bhp).
- `Seats`: Number of seats in the car.
- `Price`: The selling price of the car (target variable).

You can access the dataset [here](https://www.kaggle.com/code/sagargupta323/used-car-price-prediction) (replace this with the actual link to your dataset).

## Features

### Independent Variables (Features):
- `Name`: The car's make and model.
- `Location`: The city where the car is sold.
- `Year`: Year of manufacture.
- `Kilometers_Driven`: Total kilometers driven.
- `Fuel_Type`: Type of fuel used (CNG, Diesel, Petrol).
- `Transmission`: Manual or automatic transmission.
- `Owner_Type`: First-hand or second-hand ownership.
- `Mileage`: Car's mileage in km/kg or kmpl.
- `Engine`: Engine displacement in cubic centimeters (CC).
- `Power`: Engine power in brake horsepower (bhp).
- `Seats`: Number of seats in the car.

### Dependent Variable (Target):
- `Price`: The selling price of the car.

## Installation

To run this project locally, please ensure that you have Python installed. Then, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/sweta12232/used-car-price-prediction.git
    ```
2. Navigate to the project directory:
    ```bash
    cd used-car-price-prediction
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Modeling Process

1. **Data Preprocessing**: Handle missing values, perform categorical encoding (using one-hot encoding or label encoding), and apply feature scaling (e.g., standardization or normalization).
2. **Exploratory Data Analysis (EDA)**: Visualize the relationships between different features and car prices using libraries like `matplotlib` and `seaborn`.
3. **Model Selection**: Tried Linear Regression machine learning algorithms
4. **Model Training**: Split the data into training and test sets. Trained the models using cross-validation to evaluate performance.
5. **Evaluation**: Evaluated the models using metrics like:
   - Mean Squared Error (MSE)
   - R-squared

## Results

- Best model: `Random Forest Regressor` (or the model you selected)
- **R² Score**: 0.82
- **Mean Squared Error**: 0.1331

These results indicate that the model can predict used car prices with a high degree of accuracy.

## Future Improvements

- **Model Improvement**: Experiment with Random Forest and Gradient Boosting
- **Hyperparameter Tuning**: Optimized model hyperparameters using techniques like GridSearchCV or RandomizedSearchCV.


## Contributing

Feel free to contribute to this project by submitting pull requests. If you encounter any issues, please open an issue in this repository.

.

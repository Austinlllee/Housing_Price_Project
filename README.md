# Project 2: Housing Price Prediction

## Author: Austin Lee

### Date: 2023-04-20

---

## Overview

This project explores the prediction of housing prices using multiple linear regression models applied to the California Housing dataset. The dataset contains information about various features of California's housing market, including median income, population, and housing median age. The goal is to predict the `median_house_value` (target variable) based on these features.

The project involves:
- **Data Import and Cleaning**: Loading and preparing the dataset for analysis.
- **Model Building**: Building several regression models to predict housing prices.
- **Model Evaluation**: Assessing model performance using cross-validation.
- **Residual Analysis**: Diagnosing model assumptions using residuals.
- **Visualizations**: Plotting data and model diagnostics for better understanding.

---

## Data

The dataset used in this project is the California Housing dataset, sourced from [Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow](https://github.com/ageron/handson-ml). It contains information such as:
- `median_income`: The median income in each block group.
- `total_rooms`: The total number of rooms in the block group.
- `population`: The total population of the block group.
- `housing_median_age`: The median age of houses in the block group.
- `median_house_value`: The target variable, which we are trying to predict.

---

## Libraries Used

```r
# Helper packages
library(tidyverse)  # For data manipulation and visualization
library(reshape2)   # For reshaping data
library(dplyr)      # For data manipulation
library(ggplot2)    # For plotting

# Modeling process packages
library(rsample)    # For resampling techniques
library(caret)      # For model training and cross-validation

# Model interpretability packages
library(vip)        # For variable importance plots

# MLB Win Probability Predictor

## Project Overview

The MLB Win Probability Predictor is a machine learning project aimed at predicting the probability of one Major League Baseball (MLB) team winning against another based on their ELO ratings and other performance metrics. This project utilizes advanced machine learning techniques to provide accurate predictions, which can be useful for sports analysts, enthusiasts, and bettors.

## Features

- **Data Preprocessing**: Efficient data cleaning and preprocessing to handle missing values and prepare the dataset for modeling.
- **Feature Selection**: Use of Lasso regression for selecting important features that significantly contribute to the prediction accuracy.
- **Model Training**: Implementation of the LightGBM (LGBM) model, chosen through AutoML for its superior performance in regression tasks.
- **User Interface**: An interactive UI built using Jupyter Notebook and `ipywidgets` that allows users to select two MLB teams and see their win probabilities.
- **ELO Rating to Win Probability Conversion**: Conversion of ELO ratings to win probabilities using a logistic function for intuitive and meaningful predictions.

## Technical Details

- **Language**: Python
- **Libraries**:
  - `pandas` for data manipulation
  - `numpy` for numerical operations
  - `sklearn` for machine learning utilities
  - `flaml` for AutoML
  - `lightgbm` for the LGBM model
  - `ipywidgets` for building the interactive user interface
  - `joblib` for saving and loading models

## How It Works

1. **Data Loading**: Load and concatenate the latest and historical MLB ELO datasets.
2. **Data Cleaning**: Handle missing values by filling them with means or dropping rows where necessary.
3. **Feature Selection**: Apply Lasso regression to select the most impactful features for prediction.
4. **Model Training**: Train an LGBM model using the selected features and evaluate its performance using Mean Squared Error (MSE).
5. **Model Saving**: Save the trained model for future use.
6. **Interactive UI**: Provide an easy-to-use interface for users to select teams and view win probabilities, with results color-coded for clarity.

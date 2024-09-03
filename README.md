### Student Performance Prediction Project

## Project Overview

This project aims to predict student performance based on various features such as gender, race/ethnicity, parental level of education, lunch type, test preparation course, and scores in reading and writing. The project involves building a machine learning pipeline to process and analyze the data, and deploying the model using a Flask application.

## Project Structure


## Components

### 1. Data Ingestion

The `data_ingestion.py` script reads the dataset, splits it into training and test sets, and saves them to the `artifacts` directory. It performs the following tasks:
- Reads the raw dataset.
- Splits the data into training and test sets.
- Saves the datasets for further processing.

### 2. Data Transformation

The `data_transformation.py` script preprocesses the data by handling missing values, encoding categorical features, and scaling numerical features. It utilizes:
- `ColumnTransformer` for applying different preprocessing pipelines to numerical and categorical data.
- Saves the preprocessing object to be used in the prediction pipeline.

### 3. Model Trainer

The `model_trainer.py` script trains multiple regression models and selects the best one based on performance metrics. It includes:
- Training models such as Random Forest, Decision Tree, Gradient Boosting, XGBRegressor, CatBoostRegressor, and AdaBoost Regressor.
- Evaluating model performance using metrics like R2 score.
- Saving the best model for prediction.

### 4. Prediction Pipeline

The `predict_pipeline.py` script handles the prediction process. It includes:
- Loading the trained model and


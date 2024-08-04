# Forest Cover Type Prediction

## Overview

This project focuses on predicting forest cover types using machine learning techniques. By leveraging various features from the forestry dataset, we aim to classify land into different cover types. The project blends environmental science with data analytics, showcasing the application of machine learning in understanding and predicting forest cover.

## Dataset

The dataset includes the following features:
- **Id:** Unique identifier for each record
- **Elevation:** Elevation in meters
- **Aspect:** Aspect of the slope in degrees
- **Slope:** Slope in degrees
- **Horizontal Distance to Hydrology:** Horizontal distance to nearest water source
- **Vertical Distance to Hydrology:** Vertical distance to nearest water source
- **Soil Type:** Type of soil present
- **Cover Type:** The target variable representing different forest cover types

## Project Steps

### 1. Data Exploration

- **Import Libraries:** Utilized essential libraries including NumPy and Pandas.
- **Read Data:** Loaded the dataset to understand its structure and content.
- **Initial Inspection:**
  - Used `df.info()` to gather dataset information.
  - Checked for null values with `df.isnull().sum()`.
  - Identified duplicated values using `df.duplicated().sum()`.
  - Examined the statistical summary of the data with `df.describe()`.

### 2. Data Preprocessing

- **Data Splitting:** Utilized `sklearn.model_selection` to split the dataset into training and testing sets.
- **Standardization:** Applied `StandardScaler` to fit and transform the training data, and to transform the testing data.

### 3. Model Building and Evaluation

- **Model Training:** Employed different classifiers to build and evaluate models:
  - Logistic Regression
  - Decision Tree Classifier
  - Random Forest Classifier
- **Cross-Validation:** Used `ShuffleSplit` for robust evaluation and model validation.

### 4. Model Persistence

- **Model Saving:** Imported the `pickle` library to save the model with the highest accuracy for future use.

### 5. Deployment

- **Real-Time Prediction:** Utilized the `PIL` library to import images and `Streamlit` to deploy the model, allowing real-time predictions based on user input.

## Technologies and Libraries Used

- Python
- NumPy
- Pandas
- scikit-learn
- StandardScaler
- Logistic Regression
- DecisionTreeClassifier
- RandomForestClassifier
- pickle
- PIL
- Streamlit

## Results and Insights

The project successfully classifies forest cover types using various machine learning models. The deployed app allows users to input data and receive real-time predictions, providing an interactive tool for understanding forest cover types.



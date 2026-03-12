# IIMSTC-Water-Potability-Classification-
A machine learning project to classify water sources as safe or unsafe using chemical sensor data and heavy metal concentration, supporting public safety and clean water initiatives.
# Clean Water Potability Prediction 💧

## Project Overview

This project uses Machine Learning techniques to predict whether water
is safe (potable) or unsafe (non-potable) for drinking based on
different water quality parameters.

The model analyzes various chemical properties of water such as pH,
hardness, solids, chloramines, sulfate, conductivity, organic carbon,
trihalomethanes, and turbidity to determine potability.

The goal of this project is to help in automated water quality
monitoring and support decision-making for safe drinking water.

------------------------------------------------------------------------

# Dataset

The dataset used in this project is the Water Potability Dataset.

## Features

  Feature           Description
  ----------------- ----------------------------------------
  pH                Acidity or alkalinity of water
  Hardness          Capacity of water to precipitate soap
  Solids            Total dissolved solids
  Chloramines       Amount of chloramines in water
  Sulfate           Sulfate concentration
  Conductivity      Electrical conductivity of water
  Organic_carbon    Amount of organic carbon
  Trihalomethanes   Concentration of THMs
  Turbidity         Clarity of water
  Potability        Target variable (1 = Safe, 0 = Unsafe)

------------------------------------------------------------------------

# Technologies Used

## Programming Language

-   Python

## Libraries

-   Pandas
-   NumPy
-   Matplotlib
-   Seaborn
-   Scikit-learn
-   XGBoost
-   LightGBM
-   Imbalanced-learn (SMOTE)

------------------------------------------------------------------------

# Project Workflow

## 1. Data Loading

``` python
data = pd.read_csv("water_potability.csv")
```

## 2. Data Exploration

Basic dataset analysis includes: - Dataset shape - Data types -
Statistical summary - Missing values - Duplicate rows

## 3. Data Visualization

Visualizations used: - Potability distribution - Feature histograms -
Correlation heatmap - Box plots

Libraries used: - Matplotlib - Seaborn

## 4. Handling Missing Values

Missing values are handled using KNN Imputer.

## 5. Data Preprocessing

### Standardization

``` python
StandardScaler()
```

### Feature Engineering

``` python
PolynomialFeatures()
```

## 6. Handling Imbalanced Dataset

SMOTE (Synthetic Minority Oversampling Technique) is used to balance the
dataset.

``` python
SMOTE()
```

## 7. Train Test Split

Dataset is divided into training and testing sets.

``` python
train_test_split()
```

## 8. Machine Learning Models Used

-   Logistic Regression
-   Random Forest
-   XGBoost
-   LightGBM

## 9. Model Optimization

Hyperparameter tuning is performed using GridSearchCV with Stratified
K-Fold Cross Validation.

## 10. Model Evaluation

Models are evaluated using:

-   Accuracy
-   Precision
-   Recall
-   F1 Score
-   Confusion Matrix

------------------------------------------------------------------------

# How to Run the Project

## Step 1: Install required libraries

``` bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost lightgbm imbalanced-learn
```

## Step 2: Upload dataset

    water_potability.csv

## Step 3: Run the notebook

    Clean_Water.ipynb

------------------------------------------------------------------------

# Applications

-   Smart water quality monitoring
-   IoT water testing systems
-   Government water safety systems
-   Environmental data analysis
-   Public health monitoring

------------------------------------------------------------------------

# Future Improvements

-   Deploy as a web application
-   Real-time IoT sensor integration
-   Build API for predictions
-   Create dashboard visualization

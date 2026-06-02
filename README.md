# CodeAlpha_Car-Price-Prediction

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-orange?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-blue?logo=numpy)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-f7931e?logo=scikitlearn)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![Status](https://img.shields.io/badge/Project-Completed-success)

---

##  Project Overview

This project predicts the selling price of used cars using Machine Learning techniques. The model analyzes multiple vehicle-related features such as present price, age of the car, kilometers driven, fuel type, transmission type, and ownership history to estimate an accurate selling price.

The project also includes extensive Exploratory Data Analysis (EDA), feature engineering, model comparison, feature importance analysis, and real-world price prediction.

---

##  Project Objectives

- Analyze and understand car market data
- Perform data preprocessing and feature engineering
- Visualize trends and relationships in car pricing
- Train multiple regression models
- Compare model performance using evaluation metrics
- Predict the selling price of used vehicles

---

##  Dataset Features

| Feature | Description |
|----------|-------------|
| Car_Name | Name of the car |
| Year | Manufacturing year |
| Selling_Price | Selling price of the car (Target Variable) |
| Present_Price | Current ex-showroom price |
| Driven_kms | Total kilometers driven |
| Fuel_Type | Petrol, Diesel, or CNG |
| Selling_type | Dealer or Individual |
| Transmission | Manual or Automatic |
| Owner | Number of previous owners |

---

##  Feature Engineering

To improve prediction performance, several domain-based features were created:

###  Car Age

```python
Car_Age = Current_Year - Year
```

Represents the age of the vehicle.

### 🛣️ Kilometers Driven Per Year

```python
Kms_per_year = Driven_kms / (Car_Age + 1)
```

Measures vehicle usage intensity.

###  Brand Goodwill

```python
Brand_good_will = Selling_Price / Present_Price
```

Represents how well a vehicle retains its value over time.

---

##  Exploratory Data Analysis (EDA)

The following analyses were performed:

- Dataset structure analysis
- Missing value detection
- Statistical summary
- Feature distribution analysis
- Correlation analysis
- Categorical feature analysis

### Visualizations

- Selling Price Distribution
- Present Price Distribution
- Fuel Type Analysis
- Transmission Analysis
- Ownership Distribution
- Correlation Heatmap
- Actual vs Predicted Plot
- Residual Analysis
- Feature Importance Visualization

---

##  Machine Learning Models Used

Three regression algorithms were trained and evaluated:

### 1️ Linear Regression

A baseline regression model for price prediction.

### 2️ Decision Tree Regressor

Captures non-linear relationships in the dataset.

### 3️ Random Forest Regressor

An ensemble learning model that combines multiple decision trees for improved accuracy.

---

##  Machine Learning Workflow

```text
Data Collection
        ↓
Data Preprocessing
        ↓
Feature Engineering
        ↓
Exploratory Data Analysis
        ↓
Encoding & Scaling
        ↓
Train-Test Split
        ↓
Model Training
        ↓
Model Evaluation
        ↓
Model Comparison
        ↓
Price Prediction
```

---

##  Model Evaluation Metrics

The models were evaluated using:

- R² Score
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)

---

##  Best Model Performance

### Random Forest Regressor

| Metric | Score |
|----------|---------|
| R² Score | 0.9797 |
| MAE | 0.3982 |
| RMSE | 0.6835 |

The Random Forest Regressor achieved the highest prediction accuracy and outperformed the other models.

---

##  Feature Importance Analysis

The Random Forest model was used to identify the most influential features affecting car prices.

Key factors included:

- Present Price
- Car Age
- Kilometers Driven
- Fuel Type
- Transmission Type
- Ownership History

---

##  New Car Price Prediction

The trained model can estimate the selling price of a new vehicle by providing:

- Present Price
- Vehicle Age
- Kilometers Driven
- Fuel Type
- Selling Type
- Transmission Type
- Ownership Details

---

##  Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Jupyter Notebook

---

##  Project Structure

```text
Car-Price-Prediction/
│
├── Car Price Prediction.ipynb
├── car data.csv
├── README.md
├── requirements.txt
└── images/
```

---


##  Results

The project successfully developed a machine learning model capable of predicting used car prices with high accuracy.

The Random Forest Regressor achieved an R² Score of **0.9797**, demonstrating excellent predictive performance and strong generalization capability.

---

##  Future Improvements

- Hyperparameter Tuning
- Cross Validation
- XGBoost Regressor
- Model Deployment using Streamlit
- Real-Time Car Price Prediction Web App

---

##  Author

### Aditi Singh

M.Sc. Mathematics | Data Science Enthusiast | Machine Learning Learner
---

##  Support

If you found this project useful, please consider giving it a ⭐ on GitHub.

Your support motivates future improvements and new projects!

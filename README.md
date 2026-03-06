# Bulldozer Price Prediction using Machine Learning 🚜

This project demonstrates a **Machine Learning regression model** to predict the **sale price of bulldozers** using historical auction data.

The goal is to analyze machine characteristics and past sales data to build a model that can accurately estimate future bulldozer sale prices.

---

# Project Overview

Predicting equipment prices is useful for:
- Equipment dealers
- Construction companies
- Auction platforms
- Financial analysts

In this project we perform:
- Data exploration
- Feature engineering
- Time-series preprocessing
- Model training
- Model evaluation

---

# Problem Definition

How well can we predict the **future sale price of a bulldozer**, given its characteristics and previous examples of how similar bulldozers have been sold?

---

# Dataset

The dataset comes from the Kaggle competition:

**Bluebook for Bulldozers**

https://www.kaggle.com/c/bluebook-for-bulldozers/data

The dataset contains information about bulldozer sales including:

- Machine ID
- Model information
- Machine age
- Usage hours
- Product size
- State of sale
- Machine configuration
- Sale date
- Sale price

---

# Dataset Files

| File | Description |
|-----|-------------|
| Train.csv | Training data (up to 2011) |
| Valid.csv | Validation data (Jan 2012 – Apr 2012) |
| Test.csv | Test data (May 2012 – Nov 2012) |

Note: Due to GitHub file size limits, datasets are **not included in this repository**.

Download them from Kaggle and place them inside the `data/` folder.

---

# Evaluation Metric

The model is evaluated using:

**RMSLE (Root Mean Squared Log Error)**

RMSLE penalizes underestimates and overestimates proportionally and is commonly used in price prediction problems.

Lower RMSLE indicates better performance.

---

# Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## Project Workflow

### 1 Data Loading
- Import datasets using pandas
- Parse date columns

### 2 Data Exploration
- Understand dataset structure
- Check missing values
- Visualize price distribution

### 3 Feature Engineering
Extract time-based features from `saledate`

- saleYear
- saleMonth
- saleDay
- saleDayOfWeek
- saleDayOfYear

### 4 Data Cleaning
- Handle missing values
- Convert categorical variables

### 5 Model Training
Train regression models to predict sale price.

### 6 Model Evaluation
Evaluate using RMSLE to measure prediction accuracy.

---

## Project Structure

```
Bulldozer-Price-Prediction
│
├── bulldozer-price-prediction.ipynb
├── README.md
├── .gitignore
│
└── data/    (dataset not included)
```

---

## Installation

Clone the repository

```
git clone https://github.com/DevSen101/Bulldozer-Price-Prediction.git
```

Navigate to project folder

```
cd Bulldozer-Price-Prediction
```

---

## Example Libraries Used

```
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import sklearn
```

---

## Key Learning Points

This project demonstrates:

- Handling large real-world datasets
- Feature engineering for time-series data
- Working with missing values
- Building regression models
- Evaluating ML models using RMSLE

---


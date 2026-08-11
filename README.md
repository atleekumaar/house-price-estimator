# House Price Prediction

A machine learning project that predicts residential property valuations using XGBoost Regression based on key features such as location metrics, property specifications, and economic factors.

---

## 📌 Project Overview

This project builds an end-to-end Machine Learning pipeline using Python to predict house prices using the Boston Housing Dataset. It implements data cleaning, feature correlation analysis, train-test splitting, and evaluation using XGBoost Regressor.

---

## 🛠️ Tech Stack & Dependencies

- **Language:** Python 3.x
- **Libraries:**
  - `numpy` & `pandas` (Data Manipulation)
  - `matplotlib` & `seaborn` (Data Visualization)
  - `scikit-learn` (Data Preprocessing & Evaluation Metrics)
  - `xgboost` (Gradient Boosted Decision Trees Model)

---

## 📊 Dataset Overview

The project uses the Boston House Prices dataset containing 506 rows and 13 numerical/categorical features including:

- **CRIM:** Per capita crime rate by town
- **ZN:** Proportion of residential land zoned for large lots
- **INDUS:** Proportion of non-retail business acres
- **RM:** Average number of rooms per dwelling
- **AGE:** Proportion of owner-occupied units built prior to 1940
- **DIS:** Weighted distances to employment centres
- **TAX:** Full-value property-tax rate
- **PTRATIO:** Pupil-teacher ratio by town
- **LSTAT:** Percentage of lower status population
- **price (Target):** Median value of owner-occupied homes (in $1000s)

---

## 🚀 Workflow

1. **Data Collection & Inspection:** Loaded the dataset into a Pandas DataFrame, verified data types, dimensions, and missing values.
2. **Exploratory Data Analysis (EDA):** Calculated statistical measures and constructed a correlation heatmap using Seaborn to examine feature relationships.
3. **Data Splitting:** Divided data into features ($X$) and target ($Y$), followed by an 80-20 train-test split (`random_state=2`).
4. **Model Training:** Fitted an `XGBRegressor` model on the training data.
5. **Model Evaluation:** Evaluated predictions on both training and test sets using R² score and Mean Absolute Error (MAE).

---

## 📈 Results & Performance

| Metric | Training Data | Test Data |
| :--- | :--- | :--- |
| **R² Score** | `~0.973` | `~0.912` |
| **Mean Absolute Error (MAE)** | `~1.145` | `~1.992` |

---

## 📦 How to Run

1. Clone the repository:
   ```bash
   git clone [https://github.com/atleekumaar/house-price-estimator.git](https://github.com/atleekumaar/house-price-estimator.git)
   cd house-price-estimator
2.Install required packages:
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn xgboost

 ```
 3.Run the Jupyter / Google Colab notebook:
 ```bash
   jupyter notebook "Project : House Price Prediction.ipynb"
   ```
 

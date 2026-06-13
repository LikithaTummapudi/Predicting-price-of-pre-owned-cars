# 🚗 Car Price Prediction using Machine Learning

## 📌 Project Overview

This project predicts the prices of pre-owned cars using supervised machine learning techniques. Multiple preprocessing strategies were explored to understand the impact of missing-value handling on model performance.

Two machine learning models were implemented and compared:

* Linear Regression
* Random Forest Regressor

Two dataset variants were evaluated:

1. Dataset obtained by dropping rows with missing values
2. Dataset obtained by imputing missing values

---

## 📊 Dataset

The dataset contains approximately **50,000 used car listings** with features such as:

* Vehicle age
* Brand
* Model
* Fuel type
* Power (PS)
* Kilometers driven
* Gearbox type
* Vehicle condition

After cleaning and outlier removal, the dataset was used for predictive modeling and performance comparison.

The dataset used in this project was provided as part of course material and is not sourced from Kaggle.

🔗 Dataset Download Link

👉 https://drive.google.com/file/d/1SBXoQjDM_5vvpQeHssq2VGK36TbtJS6W/view

⚠️ The dataset is hosted externally due to size and ownership considerations and is therefore not included in this repository.

---

## 🔎 Data Preprocessing

### 🧹 Approach 1: Dropping Missing Values

* Removed records containing missing values.
* Produced a cleaner dataset.
* Reduced dataset size.

### 🧪 Approach 2: Imputing Missing Values

* Filled numerical missing values using median values.
* Filled categorical missing values using the most frequent category.
* Preserved more training data.

### Additional Processing

* Removed duplicate records.
* Filtered unrealistic values for:

  * Registration Year
  * Vehicle Price
  * Engine Power
* Created a new **Age** feature from registration year and month.
* Applied one-hot encoding to categorical variables.
* Performed exploratory data analysis (EDA) and feature relationship analysis.

---

## 🤖 Machine Learning Models

### 🔹 Linear Regression

* Baseline regression model.
* Easy to interpret.
* Assumes linear relationships between variables.

### 🔹 Random Forest Regressor

* Ensemble learning method.
* Captures non-linear relationships.
* Provides stronger predictive performance.

---

## 📈 Model Evaluation

### Dataset with Missing Values Removed

| Model             | Train R² | Test R²   | RMSE      |
| ----------------- | -------- | --------- | --------- |
| Linear Regression | 0.780    | 0.757     | 0.546     |
| Random Forest     | 0.920    | **0.850** | **0.436** |

### Dataset with Missing Values Imputed

| Model             | Train R² | Test R²   | RMSE      |
| ----------------- | -------- | --------- | --------- |
| Linear Regression | 0.702    | 0.707     | 0.648     |
| Random Forest     | 0.902    | **0.827** | **0.494** |

### Baseline Comparison

| Dataset                | Baseline RMSE |
| ---------------------- | ------------- |
| Missing Values Removed | 1.127         |
| Missing Values Imputed | 1.188         |

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn

---

## 🚀 How to Run

1. Clone the repository

```bash
git clone <repository-url>
```

2. Download the dataset and place it in the project directory.

3. Install dependencies

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

4. Run the project

```bash
python car_price_prediction.py
```

---

## 📌 Key Insights

* Random Forest consistently outperformed Linear Regression across both datasets.
* The best-performing model achieved an **R² Score of 0.85** on the test set.
* Missing-value handling significantly affected model performance.
* Removing missing values resulted in slightly better predictive accuracy than imputation.
* Feature engineering and data cleaning substantially improved prediction quality.
* Ensemble methods proved more effective than traditional linear models for used-car price prediction.

---

## 🎯 Conclusion

This project demonstrates a complete machine learning workflow, including data preprocessing, exploratory data analysis, feature engineering, model training, and evaluation. Among all experiments, the Random Forest Regressor trained on the cleaned dataset achieved the strongest performance with a test **R² score of 0.85** and **RMSE of 0.436**, making it the preferred model for predicting pre-owned car prices.

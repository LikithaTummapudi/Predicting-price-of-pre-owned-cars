# 🚗 Car Price Prediction using Machine Learning

## 📌 Project Overview

This project predicts car prices using supervised machine learning techniques.
Two different missing-value handling strategies were applied, and their impact on model performance was analyzed.

### Models implemented:

Linear Regression

Random Forest Regressor

Two dataset variants:

Dataset obtained by dropping rows with missing values

Dataset obtained by imputing missing values

## 📊 Dataset

The dataset used in this project was provided as part of course material and is not sourced from Kaggle.


🔗 Dataset Download Link

👉 https://drive.google.com/file/d/1SBXoQjDM_5vvpQeHssq2VGK36TbtJS6W/view

⚠️ The dataset is hosted externally due to size and ownership considerations and is therefore not included in this repository.

## 🔎 Data Preprocessing

Two preprocessing approaches were followed:

### 🧹 Approach 1: Dropping Missing Values

Rows containing any missing values were removed.

Results in a clean dataset.

Reduces dataset size.

### 🧪 Approach 2: Imputing Missing Values

Missing numerical values were filled using statistical methods (mean/median).

Preserves dataset size.

Helps retain valuable information.

## 🤖 Machine Learning Models
### 🔹 Linear Regression

Baseline regression model

Simple and interpretable

Assumes linear relationships between features and target

### 🔹 Random Forest Regressor

Ensemble learning technique

Handles non-linear relationships

Provides better performance in most cases

## 📈 Model Evaluation

The models were evaluated using the following metrics:

R² Score

Mean Absolute Error (MAE)

Mean Squared Error (MSE)

Comparisons were made to analyze:

The effect of missing-value handling

Performance differences between models

## 🛠️ Technologies Used

Python

Pandas

NumPy

Scikit-learn

Matplotlib / Seaborn

## 🚀 How to Run the Project
1️⃣ Clone the repository
git clone <your-repository-link>

2️⃣ Download the dataset

Download the dataset from the link above.

3️⃣ Place the dataset

Place the dataset file inside the project directory (for example, in a data/ folder).

4️⃣ Run the project
python filename.py


or open the Jupyter Notebook and run all cells.

## 📌 Key Insights

Handling missing values significantly affects prediction performance.

Random Forest generally outperforms Linear Regression.

Imputation often yields better results than dropping data.

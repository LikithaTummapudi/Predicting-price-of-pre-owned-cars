🚗 Car Price Prediction using Machine Learning
📌 Project Overview

This project focuses on predicting car prices using supervised machine learning techniques. Two different approaches were used to handle missing values in the dataset, and their impact on model performance was analyzed.

The models implemented:

✅ Linear Regression

✅ Random Forest Regressor

Both models were trained and evaluated on:

Dataset after omitting rows with missing values

Dataset after imputing missing values

This allows comparison of how missing data handling affects model accuracy.

📊 Dataset

The dataset used in this project was obtained from course material and is not sourced from Kaggle.

You can download the dataset here:

👉 Dataset Link:
https://drive.google.com/file/d/1SBXoQjDM_5vvpQeHssq2VGK36TbtJS6W/view

Note: The dataset is hosted externally due to size and ownership considerations.

🔎 Data Preprocessing

Two preprocessing strategies were applied:

1️⃣ Removing Missing Values

All rows containing any missing values were dropped.

Ensures clean dataset.

May reduce dataset size significantly.

2️⃣ Imputing Missing Values

Missing numerical values were filled using statistical methods (e.g., mean/median).

Preserves dataset size.

Reduces data loss.

🤖 Models Used
🔹 Linear Regression

Baseline regression model.

Simple and interpretable.

Useful for understanding linear relationships between features and target.

🔹 Random Forest Regressor

Ensemble learning method.

Handles non-linearity well.

Generally provides better prediction performance.

📈 Model Comparison

The models were evaluated on:

R² Score

Mean Absolute Error (MAE)

Mean Squared Error (MSE)

This comparison helps determine:

Whether imputing or dropping missing values yields better results.

Which model performs best for car price prediction.

🛠️ Technologies Used

Python

Pandas

NumPy

Scikit-learn

Matplotlib / Seaborn (for visualization)

🚀 How to Run the Project

Clone this repository:

git clone <your-repository-link>


Download the dataset from the Google Drive link above.

Place the dataset file inside the project directory.

Run the Jupyter Notebook or Python script:

python filename.py

📌 Key Insights

Handling missing data significantly impacts model performance.

Random Forest generally performs better due to its ability to model complex relationships.

Imputation often preserves predictive power compared to simply dropping data.

📬 Future Improvements

Hyperparameter tuning

Feature engineering

Cross-validation

Trying advanced models (XGBoost, Gradient Boosting)

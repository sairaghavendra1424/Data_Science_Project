# Data_Science_Project
# Predictive Maintenance and Anomaly Detection in Aircraft Engines

## 📌 Project Overview
This project focuses on predicting the Remaining Useful Life (RUL) of aircraft engines and detecting anomaly patterns using multivariate sensor data from the NASA CMAPSS dataset.

The goal is to compare statistical and machine learning approaches for predictive maintenance and evaluate their effectiveness in modelling engine degradation.

---

## 📊 Dataset
- **Source:** NASA CMAPSS Dataset  
- **Subset Used:** FD001  
- **Type:** Multivariate time-series sensor data  

The dataset includes:
- Engine ID and cycle information  
- 3 operational settings  
- 21 sensor measurements  

📎 Dataset Link:  
https://www.kaggle.com/datasets/behrad3d/nasa-cmaps  

---

## ⚙️ Project Workflow

1. **Data Loading & Cleaning**
   - Structured raw CMAPSS data
   - Removed non-informative features

2. **RUL Calculation**
   - Computed Remaining Useful Life for training data

3. **Preprocessing**
   - Feature scaling (MinMaxScaler)
   - Feature selection

4. **Exploratory Data Analysis**
   - Sensor degradation trends
   - Correlation analysis
   - PCA visualization

5. **Model Development**
   - Linear Regression
   - Random Forest
   - Gradient Boosting
   - XGBoost

6. **Feature Engineering**
   - Lag features
   - Rolling mean features

7. **Hyperparameter Tuning**
   - RandomizedSearchCV on XGBoost

8. **Anomaly Detection**
   - PCA-based anomaly detection
   - Isolation Forest

---

## 🤖 Models Used

| Model | Purpose |
|------|--------|
| Linear Regression | Baseline |
| Random Forest | Ensemble learning |
| Gradient Boosting | Sequential boosting |
| XGBoost | Optimized boosting |
| PCA | Statistical anomaly detection |
| Isolation Forest | ML-based anomaly detection |

---

## 📈 Results Summary

- **Best RMSE:** Linear Regression (~32.04)
- **Best MAE:** Gradient Boosting (~23.22)
- Feature engineering did not significantly improve performance
- Hyperparameter tuning gave minor improvements
- Anomaly detection showed increasing abnormal patterns near failure

---

## 📊 Key Insights

- Dataset shows relatively structured degradation patterns  
- Simple models can perform competitively  
- Model performance is influenced more by data than complexity  
- Anomaly detection complements RUL prediction  

---

## 🚀 Future Work

- Implement deep learning models (LSTM, RNN)  
- Use datasets with multiple operating conditions  
- Improve feature engineering techniques  
- Evaluate anomaly detection with labelled data  

---

## 🛠️ Technologies Used

- Python  
- Pandas, NumPy  
- Scikit-learn  
- XGBoost  
- Matplotlib, Seaborn  

---

## 📁 Project Structure

├──Nasa_CMaps_Data.zip
|── Data_Science_Project_SR.ipynb
├── images
├── README.md
├── LICENSE

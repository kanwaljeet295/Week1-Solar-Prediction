
# ☀️ AI Solar Energy Prediction Project (Week 1)

## 📌 Overview

This project is the Week 1 submission for the AICTE / Edunet Internship.

The goal for this week was to perform a complete "model bake-off" as shown in the tutorials. The workflow included data preprocessing, feature engineering, and training a baseline LinearRegression model. As the improvisation, advanced models (RandomForest and XGBoost) were also trained and evaluated to find the highest-performing model for this dataset.

---

## 📂 Repository Structure (Week 1)

```
Week1-Solar-Prediction/
│
├── SolarPrediction.csv             # The raw dataset used for this project
├── Week1_Project.ipynb             # Jupyter Notebook with all analysis & models
│
├── week1_scaler.pkl                # The saved data scaler
└── week1_best_model.pkl            # The saved *best* model (XGBoost)
```

This repository contains the full Week 1 project. This model will be tuned in Week 2.

---

## ⚙️ Week 1 Workflow

### 1. Data Preprocessing

Loaded the SolarPrediction.csv dataset.

Corrected a KeyError by combining Data and Time into a single DATE_TIME index.

### 2. Feature Engineering

Engineered new time-based features: Month, Day, Hour.

Engineered a Daylight_Hours feature by calculating the time between TimeSunRise and TimeSunSet.

### 3. Model Bake-Off (Improvisation)

Baseline: Trained a LinearRegression model.

Advanced: Trained RandomForestRegressor and XGBRegressor models.

### 4. Evaluation

Compared the R-squared (R2) score of all three models to find the clear winner.

The best model (RandomForest) and the data scaler were saved for future use.

---

## 📊 Key Results (Week 1)

Baseline Model (LinearRegression): R2 Score ≈ 0.62

Improvisation Model (Random Forest): R2 Score ≈ 0.93

Alternate Model (XGBoost): R2 Score ≈ 0.93

This process shows a clear performance improvement of nearly 30% by using advanced models, demonstrating a complete end-to-end process as taught in the Week 1 tutorial.

The best model (Random Forest) was selected based on its high R² score and efficiency. Although an ensemble of Random Forest and XGBoost gave slightly higher accuracy, the gain was marginal and not worth the added complexity for this stage.

---

## 🚀 How to Run

Clone the repository:

```bash
git clone https://github.com/kanwaljeet295/Week1-Solar-Prediction.git
cd Week1-Solar-Prediction
```

Install dependencies:  
(Ensure you have the libraries listed in the 'Requirements' section)

Open the notebook:  
Open and run Week1_Project.ipynb from top to bottom to reproduce all results.

---

## 📦 Requirements

- pandas  
- numpy  
- matplotlib  
- scikit-learn  
- xgboost  
- joblib

---

## ✨ Author

Kanwaljeet Singh  
B.Tech ECE  
Project completed under AICTE / Edunet Internship
```
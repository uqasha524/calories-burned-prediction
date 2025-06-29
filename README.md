# 🔥 Calories Burned Prediction Using ML & ANN

## 📌 Project Overview
This project predicts the number of calories burned during a workout based on user inputs like **age**, **weight**, **height**, **duration**, and **gender**. It compares traditional Machine Learning algorithms with **Artificial Neural Networks (ANN)** — with ANN showing superior performance.

---

<img src="Images/main.png" alt="Calories Burned Demo" width="600"/>

---

## 📊 Dataset Overview

The dataset used for this project contains biometric and workout-related features of individuals. Below is a preview of the first few rows:

| User_ID   | Gender | Age | Height | Weight | Duration | Heart_Rate | Body_Temp | Calories |
|-----------|--------|-----|--------|--------|----------|------------|-----------|----------|
| 14733363  | male   | 68  | 190.0  | 94.0   | 29.0     | 105.0      | 40.8      | 231.0    |
| 14861698  | female | 20  | 166.0  | 60.0   | 14.0     | 94.0       | 40.3      | 66.0     |
| 11179863  | male   | 69  | 179.0  | 79.0   | 5.0      | 88.0       | 38.7      | 26.0     |
| 16180408  | female | 34  | 179.0  | 71.0   | 13.0     | 100.0      | 40.5      | 71.0     |
| 17771927  | female | 27  | 154.0  | 58.0   | 10.0     | 81.0       | 39.8      | 35.0     |

Each row represents one workout session with corresponding physiological data and calories burned.

---

## 🧪 Libraries Used
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `tensorflow` / `keras`

---

## ⚙️ Python Compatibility
**Required Python version:** `3.9` to `3.12`  
> ⚠️ TensorFlow is not compatible with versions newer than 3.12.

---

## 📁 Project Structure

```plaintext
calories-prediction/
├── data/
│   ├── exercise.csv         # Input features with User_ID
│   ├── calories.csv         # Target values (calories burned) with User_ID
│   └── (Merged during runtime using pd.merge on 'User_ID')
│
├── models/
│   ├── best_model.keras     # Trained ANN model
│   ├── gender_encoder.pkl   # Label encoder for gender feature
│   └── scaler.pkl           # Preprocessing scaler used in training
│
├── notebooks/
│   └── code.ipynb           # Full workflow: EDA → Preprocessing → Training → Prediction
│
├── requirements.txt         # Python dependencies
└── README.md                # Project documentation

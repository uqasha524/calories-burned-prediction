# 🔥 Calories Burned Prediction Using ML & ANN

## 📌 Project Overview
This project predicts the number of calories burned during a workout based on user inputs like **age**, **weight**, **height**, **duration**, and **gender**. It compares traditional Machine Learning algorithms with **Artificial Neural Networks (ANN)** — with ANN showing superior performance.

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

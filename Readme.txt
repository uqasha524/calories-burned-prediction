Calories Prediction Using ML or ANN
===================================

📌 Project Description:
-----------------------
This project predicts the number of calories burned during a workout based on user inputs such as age, weight, height, workout duration, and gender. It uses both traditional Machine Learning and Artificial Neural Networks (ANN), with ANN providing better accuracy in our case.

🧪 Libraries Used:
------------------
- pandas
- numpy
- matplotlib
- scikit-learn
- tensorflow / keras
- Seaborn

⚠️ Python Version Requirement:
------------------------------
Use Python version 3.9 to 3.12 only. TensorFlow is not supported in versions newer than 3.12.

📁 Project Structure:
---------------------
calories-prediction/
│
├── data/
│   ├── exercise.csv        -> Input features with user IDs
│   ├── calories.csv        -> Target variable (calories burned) with user IDs
│     -> Merged dataset using pd.merge on 'User_ID'
│
├── models/
│   ├── best_model.keras    -> Trained ANN model file
│   ├── gender_encoder.pkl  -> Label encoder for gender
│   └── scaler.pkl          -> Scaler used during preprocessing
│
├── notebooks/
│   └── code.ipynb          -> Jupyter notebook containing full pipeline:
│                              - EDA
│                              - Data Preprocessing
│                              - Model Training
│                              - Real-Time Prediction
│
├── requirements.txt        -> Python library dependencies
└── README.txt              -> Project documentation (this file)

🔧 How to Run:
--------------
1. Clone the Repository:
   git clone https://github.com/uqasha524/calories-burned-prediction.git
   cd calories-prediction

2. Install Dependencies:
   Make sure you're using Python 3.9 to 3.12, then run:
   pip install pandas numpy matplotlib scikit-learn tensorflow seaborn


3. Open the Notebook:
   Open notebooks/code.ipynb using Jupyter Notebook or VS Code.
   It contains all steps from EDA to real-time calorie prediction.

✅ Notes:
---------
- The ANN model (best_model.keras) gave better accuracy than traditional ML models.
- Ensure gender_encoder.pkl and scaler.pkl are loaded correctly during prediction.

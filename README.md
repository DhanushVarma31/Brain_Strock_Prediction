# Brain_Strock_Prediction

# Brain_stroke_prediction

# 🧠 Brain Stroke Prediction using Machine Learning

## 📌 Project Overview
This project focuses on predicting the likelihood of a brain stroke using Machine Learning techniques. Early detection of stroke risk is crucial in healthcare, and this model aims to assist in identifying high-risk patients based on medical and demographic data.

---

## 🎯 Objective
- Predict whether a patient is at risk of stroke (0 = No, 1 = Yes)
- Handle imbalanced medical dataset effectively
- Evaluate model performance using multiple metrics
- Identify important features contributing to stroke risk

---

## 📊 Dataset Information
- **Dataset Name:** Stroke Prediction Dataset
- **Source:** Kaggle
- **Total Records:** 5110
- **Features:** 12

### Key Features:
- Age
- Gender
- BMI
- Average Glucose Level
- Hypertension
- Heart Disease
- Smoking Status
- Work Type
- Residence Type

### Target Variable:
- `stroke` → (0 = No Stroke, 1 = Stroke)

---

## ⚙️ Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn (SMOTE)

---

## 🔄 Project Workflow

1. **Data Loading**
2. **Data Exploration**
3. **Handling Missing Values (BMI → Median)**
4. **Label Encoding for categorical features**
5. **Train-Test Split (80/20 with stratification)**
6. **Handling Imbalance using SMOTE**
7. **Model Training (Random Forest)**
8. **Model Evaluation**
9. **Visualization (Confusion Matrix, ROC Curve, Feature Importance)**

---

## 🤖 Model Used

### Random Forest Classifier
- `n_estimators = 200`
- `max_depth = None`
- `class_weight = 'balanced'`
- `random_state = 42`

### Why Random Forest?
- Handles mixed data types
- Reduces overfitting
- Works well with tabular data
- Provides feature importance

---

## 📈 Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC Score

---

## 📊 Results Summary

| Metric      | Value (Approx) |
|------------|---------------|
| Accuracy   | ~90%          |
| Precision  | Low (due to imbalance) |
| Recall     | Low for stroke class |
| ROC-AUC    | Moderate      |

### Key Observation:
- Model performs well for **non-stroke cases**
- Needs improvement for **stroke detection (minority class)**

---

## 📉 Confusion Matrix Interpretation

- True Negative (TN): Correctly predicted no-stroke
- True Positive (TP): Correctly predicted stroke
- False Negative (FN): Missed stroke cases (critical)
- False Positive (FP): False alarms

---

## 📊 Visualizations

- Confusion Matrix Heatmap
- ROC Curve
- Feature Importance Graph

---

## 🔍 Feature Importance Insights

Top contributing features:
- Age
- Average Glucose Level
- BMI
- Hypertension
- Heart Disease

---

## ⚠️ Challenges

- Highly imbalanced dataset
- Low recall for stroke cases
- Limited dataset size

---

## 🚀 Future Improvements

- Hyperparameter tuning
- Use advanced models like XGBoost
- Increase dataset size
- Deploy using Flask or Streamlit
- Improve recall using better imbalance techniques

---

## 📂 Project Structure

├── dataset/
├── notebooks/
├── models/
├── README.md
└── brain_stroke_prediction.py

---


---

## ▶️ How to Run the Project

1. Clone the repository:  git clone https://github.com/your-username/brain-stroke-prediction.git
2. Install dependencies:  pip install -r requirements.txt
3. Run the script:   python brain_stroke_prediction.py

## 📌 Conclusion

This project demonstrates how machine learning can be applied in healthcare to predict stroke risk. While Random Forest performs well overall, improvements are needed for detecting minority stroke cases.

---

## 🙏 Acknowledgment
- Kaggle for dataset
- Scikit-learn documentation

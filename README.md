# Heart Disease Prediction ML Model

## 📌 Overview
Heart disease is one of the leading causes of mortality worldwide. Early detection and prediction can significantly improve patient outcomes.  
This project builds a **machine learning model** to predict whether a patient is at risk of heart disease based on clinical features.  

The model uses the **Kaggle Heart Disease Dataset** and compares Logistic Regression and Random Forest.  
Random Forest achieved the best performance with very high accuracy and ROC-AUC score.

---

## 📂 Dataset
- **Source:** [Kaggle Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)  
- **Records:** 1025 patients  
- **Features:** 13 clinical features (age, sex, chest pain type, cholesterol, etc.)  
- **Target:** `1 = Heart Disease Present`, `0 = No Heart Disease`

---

## ⚙️ Methodology
1. Load dataset (`heart.csv`) using pandas.  
2. Train-test split (80-20).  
3. Apply two ML models:
   - Logistic Regression  
   - Random Forest Classifier  
4. Perform 5-fold Stratified Cross-Validation with hyperparameter tuning.  
5. Evaluate models using:
   - Accuracy  
   - ROC-AUC score  
   - Confusion Matrix  
   - Classification Report  
   - ROC Curve  

---

## 📚 Libraries Used
- `pandas` – Data loading & preprocessing  
- `numpy` – Numerical operations  
- `scikit-learn` – ML modeling & evaluation  
- `matplotlib` – Visualization  

---

## 🚀 Results
- **Best Model:** Random Forest Classifier  
- **Test Accuracy:** 100%  
- **ROC-AUC Score:** 1.00  
- **Confusion Matrix:** Very few or no misclassifications  
- **ROC Curve:** Clear separation between positive & negative classes  

---

## 🏥 Conclusion
The **Random Forest model** achieved outstanding performance, making it a strong candidate for assisting in medical diagnosis.  
However, results should be validated on larger, real-world datasets to ensure generalization.  

---

## 📌 How to Run
### Option 1: Run as Python Script
```bash
python Heart_Disease_Prediction_ML_Model.py --data path/to/heart.csv

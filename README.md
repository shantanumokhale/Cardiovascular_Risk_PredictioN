# Cardiovascular Risk Prediction

---

### **Introduction:**
Early detection of coronary heart disease (CHD) is crucial for promoting preventive measures and enabling timely intervention. Identifying CHD risk early can lead to lifestyle changes, such as improved diet and increased physical activity, potentially reducing the need for more invasive treatments.

---

### **Problem Statement:**
The objective is to develop a model that can predict the risk of a patient developing CHD within the next 10 years.

---

### **Data Description:**
The dataset consists of over 4,000 records, encompassing 15 attributes that include demographic, behavioral, and medical factors.

---

### **Demographic Attributes:**
- **Sex**: Gender of the patient (male "M" or female "F")
- **Age**: Age of the patient

### **Behavioral Attributes:**
- **is_smoking**: Current smoker status ("YES" or "NO")
- **Cigs Per Day**: Average number of cigarettes smoked per day

### **Medical History Attributes:**
- **BP Meds**: On blood pressure medication
- **Prevalent Stroke**: History of stroke
- **Prevalent Hyp**: Hypertensive status
- **Diabetes**: Diabetes status

---

### **Approach:**

#### **Data Preparation:**
- Removed null values and duplicates to ensure data integrity.
- Applied SMOTE (Synthetic Minority Over-sampling Technique) and random undersampling to balance the dataset.

#### **Feature Engineering:**
- **Hypertension**: Derived from systolic and diastolic blood pressure measurements.
- **Diabetes Severity**: Derived from diabetes status and glucose levels.
- **Smoking Factor**: Created from the average daily cigarette consumption.

---

### **Conclusion:**
The application of XGBoost, combined with hyperparameter tuning through grid search and cross-validation, achieved a recall of 92%. Here’s a summary of the project:

1. **Data Cleaning**: Removed inconsistencies and prepared the data for analysis.
2. **Exploratory Data Analysis (EDA)**: Conducted to understand data distributions and relationships.
3. **Data Transformation**: Ensured the data was suitable for machine learning models.
4. **Model Building and Evaluation**: Implemented five models—Logistic Regression, Random Forest, XGB Classifier, KNN, and SVM. The Random Forest model emerged as the best-performing base model.
5. **Hyperparameter Tuning**: Enhanced the Random Forest model to improve performance further.

The final model achieved approximately 90% accuracy and precision on the test set, with a recall of around 88%.

### **Feature Importance Analysis:**
Using SHAP (SHapley Additive exPlanations), we identified the most influential features:
- **Gender**
- **Age**
- **Pulse Pressure**

### **Future Work:**
- Explore other machine learning models and techniques to enhance performance.
- Collaborate with medical experts to engineer additional features, which could further improve model accuracy.

This comprehensive approach to CHD risk prediction demonstrates the potential for machine learning to significantly impact early disease detection and preventive healthcare.

---

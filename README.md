# Cardiovascular Risk Prediction
---
Introduction:
Early prediction of coronary heart disease (CHD) is crucial for raising awareness and enabling preventive measures such as dietary changes and exercise. Detecting CHD early allows for timely treatment, potentially avoiding more invasive interventions.
---
Problem Statement:
The aim is to predict whether a patient is at risk of developing CHD within the next 10 years.
---
Data Description:
The dataset comprises over 4,000 records with 15 attributes, including demographic, behavioral, and medical factors.
---
Demographic:
- Sex: male ("M") or female ("F")
- Age: patient's age
---
Behavioral:
- is_smoking: current smoker ("YES" or "NO")
- Cigs Per Day: average daily cigarette consumption
---
Medical History:
- BP Meds: on blood pressure medication
- Prevalent Stroke: history of stroke
- Prevalent Hyp: hypertensive
- Diabetes: diabetes status
---
Approach:
Data Preparation:
- Removed null values and duplicates.
- Used SMOTE and random undersampling for dataset balancing.
---
Feature Engineering:
- Derived 'Hypertension' from systolic and diastolic blood pressure.
- Derived 'Diabetes Severity' from diabetes and glucose levels.
- Created 'Smoking Factor' from cigarette consumption.
---
Conclusion:
Utilizing XGBoost and fine-tuning parameters through grid search and cross-validation achieved a recall of 92%.
---

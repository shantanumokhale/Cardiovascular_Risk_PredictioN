![image](https://github.com/shantanumokhale/Cardiovascular_Risk_Prediction/assets/120486081/d2731c18-a0b6-4c8a-8540-882454ee165d)
### Problem Statement
- **Objective:** Predict the 10-year risk of future coronary heart disease (CHD) in patients.
- **Dataset:** Cardiovascular study data from Framingham, Massachusetts.
- **Attributes:** 15 attributes, including demographic, behavioral, and medical risk factors.
- **Target Variable:** 10-year risk of CHD (binary: 1 = "Yes", 0 = "No").

![image](https://github.com/shantanumokhale/Cardiovascular_Risk_Prediction/assets/120486081/20a158f3-2ad4-4d13-97f6-175afc864734)
### Data Features
- **Demographic:**
  - **Sex:** Male or female ("M" or "F").
  - **Age:** Age of the patient (continuous).
- **Behavioral:**
  - **Is Smoking:** Current smoker status ("YES" or "NO").
  - **Cigs Per Day:** Number of cigarettes smoked per day (continuous).
- **Medical (History):**
  - **BP Meds:** On blood pressure medication (nominal).
  - **Prevalent Stroke:** History of stroke (nominal).
  - **Prevalent Hyp:** History of hypertension (nominal).
  - **Diabetes:** Diabetes status (nominal).
- **Medical (Current):**
  - **Tot Chol:** Total cholesterol level (continuous).
  - **Sys BP:** Systolic blood pressure (continuous).
  - **Dia BP:** Diastolic blood pressure (continuous).
  - **BMI:** Body Mass Index (continuous).
  - **Heart Rate:** Heart rate (continuous).
  - **Glucose:** Glucose level (continuous).

![image](https://github.com/shantanumokhale/Cardiovascular_Risk_Prediction/assets/120486081/c44596ae-1132-418d-8f4e-11b7fd397a49)
### Exploratory Data Analysis (EDA)
- **Comparisons:** Target variable CHD vs. independent variables.
- **Techniques:** Feature engineering, feature transformation, outlier handling, categorical and numerical data analysis.
- **Visualizations:** Histograms, violin plots, bar plots to analyze correlations and attribute effects on CHD.

![image](https://github.com/shantanumokhale/Cardiovascular_Risk_Prediction/assets/120486081/dc8faf9f-fd7b-437e-9ea5-bd7a8370c680)
### Data Preprocessing
- **Handling Missing Values:** Imputed with mean and mode.
- **Duplicate Values:** None found.
- **Outliers:** Imputed rather than deleted.
- **Label Encoding:** For categorical variables (sex, is smoking).

![image](https://github.com/shantanumokhale/Cardiovascular_Risk_Prediction/assets/120486081/243761a9-cf8d-4864-a59e-3f278e99d08a)
### Feature Engineering
- **Feature Selection:**
  - **Methods:** Variance threshold, chi-square tests.
  - **Outcome:** Identified and eliminated less relevant features.
- **Balancing Target Variable:**
  - **Technique:** SMOTE (Synthetic Minority Oversampling Technique).
    
![image](https://github.com/shantanumokhale/Cardiovascular_Risk_Prediction/assets/120486081/5a745afc-73ac-4093-9fe2-367edbd50677)
### Algorithms and Models
1. **Logistic Regression:**
   - **Accuracy:** 85.84%, increased to 85.98% with hyper-parameter tuning.
2. **K-Nearest Neighbors (KNN):**
   - **Accuracy:** 84.36%, increased to 85.69% with hyper-parameter tuning.
3. **Decision Tree:**
   - **Accuracy:** 74.92%, increased to 85.69% with hyper-parameter tuning.
4. **Random Forest Classifier:**
   - **Accuracy:** 84.80%.
     
![image](https://github.com/shantanumokhale/Cardiovascular_Risk_Prediction/assets/120486081/f390f704-7d38-4aa9-8e52-faa644c14880)
### Model Insights
- **Significant Features:** BP Meds, prevalent stroke, diabetes, smoking status, age, systolic and diastolic BP.
- **Multicollinearity Handling:** Retained cigsPerDay over is_smoking, retained diaBP over sysBP.
- **Variance Threshold:** Discarded features not meeting 99% variance threshold.

![image](https://github.com/shantanumokhale/Cardiovascular_Risk_Prediction/assets/120486081/99c1132e-dc54-4ce2-9d83-06cca5335bd6)
### Observations
- **Smoking:** Higher CHD risk for heavy smokers.
- **Gender:** Males smoke more, but females have higher CHD risk.
- **Age Group:** Highest CHD risk in ages 35-50.
- **Feature Irrelevance:** Education was irrelevant (identified via chi-square test).
![image](https://github.com/shantanumokhale/Cardiovascular_Risk_Prediction/assets/120486081/442b2af0-9e4f-4f13-8e44-b9c649d5ca4e)

### Challenges
- **Outliers:** 14% of data were outliers, imputed with median values.
- **Categorical Features:** Label encoded.
- **Irrelevant Features:** Adjusted for multicollinearity and low variance.
- **Imbalanced Target:** Balanced using SMOTE.
- **Complex Computations:** Required careful handling to avoid data loss.
![image](https://github.com/shantanumokhale/Cardiovascular_Risk_Prediction/assets/120486081/79bd7b60-ded0-4ecf-ba33-4114042e5f6c)

### Conclusion
- **Best Performing Models:** Logistic Regression, KNN, and Random Forest.
- **Ease of Implementation:** Logistic regression was simplest; Random Forest was time-intensive.
- **Overall Accuracy:** Models improved with hyper-parameter tuning and feature selection.
![image](https://github.com/shantanumokhale/Cardiovascular_Risk_Prediction/assets/120486081/40baf263-2109-409f-a18e-0bb23fb03532)

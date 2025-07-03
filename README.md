# Cancer-Risk-Classification
The goal of the project is to develop a machine learning classification model which is capable of predicting cancer risk based on both medical and lifestyle factors. This would allow for medical professionals to easily identify and address high risk patients.

## 📊 Dataset
The dataset used is from Kaggle:  
[🔗 Cancer Prediction Dataset](https://www.kaggle.com/datasets/rabieelkharoua/cancer-prediction-dataset/data)  
It includes 1,500 patient records with 8 features:
- Age
- Gender
- BMI
- Smoking
- Genetic Risk
- Physical Activity
- Alcohol Intake
- Cancer History

## ⚙️ Workflow
1. **Data Cleaning & Preparation**
   - Checked for missing/duplicate values and outliers.
   - Verified categorical encoding and class balance.
   - Standardised numerical features for model compatibility.

2. **Exploratory Data Analysis (EDA)**
   - Univariate and bivariate analysis performed using visualisation.
   - Identified feature-target relationships using correlation and multicollinearity checks.

3. **Feature Selection**
   - Applied statistical tests (t-test, chi-square, F-score).
   - All features retained due to statistical significance.

4. **Model Training**
   - Models used:
     - Logistic Regression (Baseline)
     - Gradient Descent Logistic Regression
     - ElasticNet Logistic Regression (with cross-validation and hyperparameter tuning)
   - Balanced class weights were tested for improved fairness.

5. **Evaluation**
   - Metrics: Accuracy, ROC-AUC, Confusion Matrix, Precision, Recall.
   - Gradient Descent Logistic Regression selected as best model with:
     - **88% accuracy**
     - **89% recall for cancer-positive cases**

## ✅ Results
- All models performed well with ROC-AUC of 0.943.
- Gradient Descent model achieved the best trade-off between recall and false positives.
- ElasticNet model showed slightly better precision but missed more cancer cases.

## 📁 Technologies Used
- Python (Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn, Statsmodels, imblearn)

## 📌 Conclusion
Gradient Descent Logistic Regression is the most suitable model for this cancer risk prediction problem due to its high recall and balanced performance, especially critical in medical decision-making scenarios.

---

**Author**: Darius Dylan Govender

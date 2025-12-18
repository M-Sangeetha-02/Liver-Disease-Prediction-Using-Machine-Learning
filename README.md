# Liver Disease Prediction using Machine Learning

##  Project Overview
This project focuses on predicting liver disease at an early stage using machine learning techniques applied to routine biochemical test data. Early diagnosis is critical, as liver disease often shows no symptoms until advanced stages.  
Using the Indian Liver Patient Dataset (ILPD), multiple classification models were evaluated to identify the most reliable and clinically useful approach.

##  Objectives
- Predict liver disease using standard blood test parameters
- Compare multiple machine learning classification algorithms
- Reduce false negatives by maximizing recall
- Identify key biochemical features influencing liver disease

---

##  Dataset
- **Source:** UCI Machine Learning Repository (Indian Liver Patient Dataset – ILPD)
- **Records:** 583 patients (Andhra Pradesh, India)
- **Features:** Age, Gender, Bilirubin levels, Liver enzymes, Proteins
- **Target:** Liver Disease (1) / No Disease (0)

## ⚙️ Methodology
1. **Data Cleaning**
   - Missing value imputation (median/mode)
   - Removal of duplicates and invalid entries

2. **Exploratory Data Analysis (EDA)**
   - Histograms, boxplots, correlation heatmaps
   - Identification of skewness, outliers, and feature relationships

3. **Preprocessing**
   - Label encoding (Gender)
   - Feature scaling using StandardScaler
   - Outlier removal using IQR method
   - Handling class imbalance using oversampling

4. **Feature Selection**
   - Random Forest feature importance
   - Selected top biochemical predictors

5. **Model Training**
   - Train–test split (80:20)
   - Hyperparameter tuning
   - Multiple classification models evaluated

##  Algorithms Used
- Logistic Regression
- Decision Tree
- Random Forest
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- AdaBoost
- Gradient Boosting
- XGBoost
- LightGBM

##  Performance Comparison

| Model | Accuracy | Precision | Recall | ROC-AUC |
|------|----------|-----------|--------|---------|
| Logistic Regression | 0.77 | 0.79 | 0.75 | 0.82 |
| Random Forest | 0.85 | 0.86 | 0.83 | 0.90 |
| XGBoost | 0.86 | 0.87 | 0.84 | 0.91 |
| **LightGBM** | **0.88** | **0.89** | **0.86** | **0.93** |

 LightGBM achieved the best overall performance  
 High recall ensured fewer false negatives, which is crucial in medical diagnosis
]

##  Key Features Identified
- Albumin
- Total Bilirubin
- Direct Bilirubin
- SGOT (AST)
- SGPT (ALT)
- Alkaline Phosphatase
- Albumin/Globulin Ratio
- Age

These features align with established medical knowledge.

##  Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- XGBoost, LightGBM
- Jupyter Notebook

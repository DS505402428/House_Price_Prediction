# House Price Prediction Project

## Overview
A comprehensive analysis of house price prediction using the Ames Housing dataset, consisting of 79 explanatory variables and 1,460 training samples. The project focuses on developing and optimizing various regression models to predict house sale prices.

---

## Dataset Information
- **Training Set**: 1,460 samples  
- **Test Set**: 1,459 samples  
- **Features**: 79 variables describing residential homes  
- **Target Variable**: Sale Price  
- **Location**: Ames, Iowa  

---

## Methodology

### Data Preprocessing
1. **Feature Categorization**:
   - Numerical and Categorical Classification  
2. **Missing Value Handling**:
   - Linear interpolation for `LotFrontage`  
   - Mode imputation for sparse missing values  
   - Label encoding for extensive missing values  
3. **Encoding**:
   - One-hot encoding for categorical variables  
4. **Target Variable Transformation**:
   - Log transformation of `Sale Price`  
5. **Train-Test Split**:
   - Implementation for validation and testing  

---

## Model Performance

| Model              | RMSE   | Standard Deviation |
|---------------------|--------|--------------------|
| Linear Regression   | 0.1664 | ±0.0326           |
| Ridge Regression    | 0.1555 | ±0.0304           |
| Lasso Regression    | 0.2022 | ±0.0413           |
| ElasticNet          | 0.1970 | ±0.0394           |
| KNN                 | 0.2324 | ±0.0129           |
| Random Forest       | 0.1496 | ±0.0124           |
| SVR                 | 0.2110 | ±0.0151           |
| Gradient Boosting   | 0.1343 | ±0.0120           |

### Best Model: Gradient Boosting Regressor
- **Optimized Parameters**:
  - `n_estimators`: 300  
  - `learning_rate`: 0.1  
  - `max_depth`: 3  
- **Final RMSE**: 0.1311 (improved from baseline 0.1343)  

---

## Key Findings
- Gradient Boosting Regressor outperformed other models  
- Hyperparameter optimization improved model performance  
- Balanced model complexity achieved through moderate learning rate and controlled tree depth  

---

## Future Improvements
1. Enhanced feature engineering  
2. Exploration of advanced ensemble methods  
3. Integration of external data sources  
4. Investigation of feature importance  
5. Implementation of deep learning approaches  

---

## Technologies Used
- **Python**  
- **Scikit-learn**  
- **Pandas**  
- **NumPy**  
- **GridSearchCV**  
- **Cross-validation Techniques**  

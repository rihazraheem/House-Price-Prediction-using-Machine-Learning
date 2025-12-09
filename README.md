# Housing Price Prediction Projects

This repository contains two projects on housing price prediction using Python and machine learning. The projects showcase my journey from basic regression modeling to advanced preprocessing and pipeline-based workflows.

---

## 1. Basic Housing Linear Regression

**Folder:** `Basic-Housing-LinearRegression/`  

**Dataset:** `Housing.csv` (545 rows, 13 columns)  

**Description:**  
- Predict housing prices using a simple **Linear Regression** model.  
- Focused on handling categorical variables using **One-Hot Encoding**.  
- Performed basic **EDA** and checked for missing values.  
- Split the data into training and testing sets and evaluated the model.  

**Key Steps:**
1. Load dataset and inspect data.
2. Handle missing values by dropping NA rows (dataset had no missing values after drop).
3. Encode categorical features using One-Hot Encoding.
4. Split data into training and testing sets.
5. Train a Linear Regression model.
6. Evaluate using **R²** and **MSE**.

**Results:**
- Mean Squared Error (MSE): 1,754,318,687,330.66  
- R-squared (R²): 0.65  

**Key Learning:**  
This project helped me understand preprocessing of categorical features and basic regression modeling.  

---

## 2. Advanced Housing Price Prediction with Pipelines

**Folder:** `Advanced-Housing-Pipeline/`  

**Dataset:** Ames Housing Dataset (`AmesHousing.csv`) with 2930 rows and 82 columns  

**Description:**  
- Used a **pipeline approach** to handle preprocessing and model training.  
- Handled missing values smartly:
  - Categorical columns → filled missing with mode  
  - Numerical columns → filled missing with median  
- Explored data using **EDA** (distributions, scatter plots, correlations).  
- Trained three models using the same preprocessing pipeline:
  1. **Linear Regression**
  2. **Random Forest Regressor**
  3. **XGBoost Regressor**  

**Key Steps:**
1. Load and inspect dataset.  
2. Handle missing values.  
3. Identify categorical and numerical columns.  
4. Build a preprocessing pipeline using `ColumnTransformer`:
   - StandardScaler for numeric features  
   - OneHotEncoder for categorical features  
5. Train models within the pipeline.  
6. Evaluate using **R²** and **RMSE**.  

**Results:**

| Model | R² | RMSE |
|-------|----|------|
| Linear Regression | 0.89 | 29,635 |
| Random Forest | 0.91 | 26,984 |
| XGBoost | 0.93 | 24,015 |

**Key Learning:**  
- Learned to handle missing values strategically.  
- Learned to use pipelines for preprocessing and model training.  
- Tree-based models (Random Forest, XGBoost) capture non-linear relationships and outperform linear regression.  
- Model evaluation metrics help compare and choose the best model.  

## Future Improvements
- Hyperparameter tuning using `GridSearchCV` or `RandomizedSearchCV`.  
- Feature engineering for better predictive power.  
- Experimenting with ensemble methods like LightGBM or CatBoost.  
- Visualizing feature importance for tree-based models.  



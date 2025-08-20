# California Housing Price Prediction  

This project demonstrates a **complete Machine Learning pipeline** applied to the **California Housing Dataset**. The goal is to predict housing prices based on demographic and geographic features.  

The notebook walks through data exploration, preprocessing, model training, and **hyperparameter tuning with Optuna**.  

---

##  Objectives  

- Perform **exploratory data analysis (EDA)** with visualizations  
- Handle missing values and categorical features  
- Train and evaluate a **Random Forest Regressor**  
- Use **Optuna** for hyperparameter tuning  
- Compare baseline and tuned model performance  

---

## Dataset  

- **File:** `housing.csv`  
- **Source:** [California Housing Prices dataset](https://www.kaggle.com/datasets/camnugent/california-housing-prices)  
- **Target:** `median_house_value` (Median house price in block groups)  

**Features:**  
- `median_income`  
- `housing_median_age`  
- `total_rooms`  
- `total_bedrooms`  
- `population`  
- `households`  
- `latitude`, `longitude`  
- `ocean_proximity` (categorical, one-hot encoded)  

---

## Workflow  

1. **Data Exploration & Visualization**  
   - Histograms of all features  
   - Correlation heatmap  
   - Scatter plots (income, age, rooms vs. price)  
   - Target distribution analysis  

2. **Preprocessing**  
   - Missing value imputation (median)  
   - Train-test split  

3. **Model Training**  
   - **Random Forest Regressor** baseline model  

4. **Evaluation Metrics**  
   - Root Mean Squared Error (RMSE)  
   - R² Score  

5. **Hyperparameter Optimization**  
   - Tuned `n_estimators`, `max_depth`, `min_samples_split`, `min_samples_leaf` using **Optuna**  
   - Improved model accuracy significantly  

---

## Results  
 
- **Tuned Random Forest Performance (Optuna best model)**  
  - Final RMSE: **48807.23**  
  - Final R2: **0.8182**  

✅ The tuned Random Forest model clearly outperformed the baseline.  


---

## Tech Stack

- Python

- Pandas, NumPy – Data manipulation

- Matplotlib, Seaborn – Visualization

- Scikit-Learn – Machine learning models & metrics

- Optuna – Hyperparameter optimization

- Jupyter Notebook


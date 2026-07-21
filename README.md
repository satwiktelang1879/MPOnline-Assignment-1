# Medical Insurance Cost Prediction using Multiple Linear Regression

## Author Details

- **Author:** SATWIK TELANG
- **Registration Number:** 23BAI11046
- **Application Number:** IN26011013
- **Batch Number:** AI/ML Internship Batch 1(A) - Nishant Shrivastava (1:00-3:00pm, Mon-Fri)
- **Email ID:** satwik.23bai11046@vitbhopal.ac.in

---

## Objective

The objective of this project is to develop a **Multiple Linear Regression** model that predicts medical insurance charges based on an individual's demographic and health-related attributes such as age, BMI, smoking status, sex, region, and number of children.

---

## Dataset

**Medical Cost Personal Insurance Dataset**

- **Source:** Kaggle
- **Dataset Link:** https://www.kaggle.com/datasets/mirichoi0218/insurance

---

## Technologies & Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Kaggle API
- Jupyter Notebook

---

## Methodology

### 1. Data Understanding
- Loaded the insurance dataset.
- Explored the dataset structure.
- Identified numerical and categorical features.
- Checked data types and target variable distribution.

### 2. Data Preprocessing
- Checked for missing values.
- Applied One-Hot Encoding on categorical variables:
  - Sex
  - Smoker
  - Region
- Used `drop_first=True` to avoid the dummy variable trap.

### 3. Train-Test Split
- Split the dataset into:
  - **80% Training Data**
  - **20% Testing Data**
- Used `train_test_split()` from Scikit-learn.

### 4. Model Development
- Implemented the **Multiple Linear Regression** model using Scikit-learn's `LinearRegression`.
- Trained the model using all available input features.

### 5. Model Evaluation
The model performance was evaluated using:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- R² Score
- Actual vs Predicted Scatter Plot

---

## Results

- **R² Score:** ~0.78
- **Primary Cost Drivers:**
  - Smoking Status
  - Age
  - BMI

The model explains approximately **78%** of the variation in insurance charges, indicating good predictive performance for a linear model.

---

## Conclusion

This project demonstrates that **Multiple Linear Regression** can effectively predict medical insurance costs using demographic and health-related information.

The model achieved an **R² Score of approximately 0.78**, showing that it captures the overall relationship between input features and insurance charges reasonably well.

However, linear regression cannot fully model complex non-linear interactions among variables, such as the combined effect of smoking and high BMI. Future improvements can be achieved by using advanced machine learning algorithms such as:

- Random Forest Regressor
- XGBoost Regressor
- Gradient Boosting
- LightGBM

These models can better capture non-linear relationships and improve prediction accuracy.

---

## Project Structure

```
Medical-Insurance-Cost-Prediction/
│
├── Assignment-1.ipynb
├── README.md
└── insurance.csv
```

---

## Output

The project generates:

- Trained Multiple Linear Regression Model
- Model Performance Metrics (MAE, MSE, R²)
- Actual vs Predicted Charges Scatter Plot
- Prediction Analysis and Conclusions

---

## License

This project is developed for academic purposes as part of the MP Online Assignment.

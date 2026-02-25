Housing Price Prediction
Comparative Machine Learning Models (Linear Regression, KNN, Decision Tree)


This project develops and compares multiple machine learning models to predict housing prices using structured real estate data.
The objective is to:
Evaluate predictive performance across different algorithms
Understand feature impact on housing prices
Apply interpretable machine learning techniques
The following models were implemented and compared:
- Linear Regression
- K-Nearest Neighbors (KNN)
- Decision Tree Regressor
All models were built within a Scikit-learn Pipeline framework to ensure clean preprocessing and reproducibility.


Business Context;
Accurate housing price estimation is critical for:
- Real estate agencies
- Property investors
- Urban planning analysts
- Buyers and sellers
By analyzing structural and locational features, this project identifies the key drivers influencing property valuation.


Dataset Overview;

Category                                Example Features
- Structural                            - area_sqm, bathrooms, age_years
- Location                              - neighborhood
- Quality/View                          - has_sea_view, sea_view_label
- Target                                - price
  

Methodology;

- Data Preprocessing
- Target variable separated (price)
- 80/20 Train-Test split
- Categorical encoding using OneHotEncoder
- Numerical features passed directly
- All transformations handled inside a ColumnTransformer
- Entire workflow encapsulated in a Pipeline


Models Implemented;

1. Linear Regression
 - Baseline interpretable model
 - Captures linear relationships
 - Useful benchmark for comparison

2. K-Nearest Neighbors (KNN)
 - Instance-based learning
 - Captures local neighborhood effects
 - Sensitive to feature scaling
  
3. Decision Tree Regressor
 - Captures nonlinear relationships
 - Automatically models interactions
 - Provides feature importance insights
 - High interpretability


Model Evaluation;

- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)
- R² Score
- Optional 5-Fold Cross Validation


Model Interpretability (SHAP);
To enhance transparency, SHAP (SHapley Additive exPlanations) was applied:
 - Global feature impact visualization
 - Individual prediction breakdown
 - Clear contribution analysis


Tech Stack
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- SHAP


Project Structure;

Housing-Price-Prediction-Data_Analysis/
│
├── Housing_Price_Prediction.ipynb
├── housing_full.csv
├── README.md
└── .venv/



Reproducibility;

1. Clone repository
2. Create virtual environment:
      python -m venv .venv
      source .venv/bin/activate
3. Install dependencies:
      pip install pandas numpy scikit-learn matplotlib seaborn shap
4. Run notebook sequentially


Key Takeaways
- Nonlinear models outperform purely linear assumptions.
- Location significantly influences property valuation.
- Feature engineering and preprocessing strongly impact performance.
- Interpretability techniques improve trust and transparency.
  

Author - Merve Uçar
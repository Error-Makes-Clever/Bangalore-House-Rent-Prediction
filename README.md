# Machine Learning Project 1  

## 🏠 Bangalore House Rent Prediction | Machine Learning Project  

This project focuses on predicting house rental prices in Bangalore using machine learning techniques. The data was **collected through web scraping** from real estate platforms, ensuring a diverse and relevant dataset for analysis. The process involves data preprocessing, exploratory data analysis (EDA), feature engineering, feature selection, and model building to accurately estimate rental costs based on factors like size, age, and amenities.  

### 🔍 Key Highlights  
- **Data Collection:** Automated web scraping from real estate websites (e.g., 99acres). The scraper uses Selenium and BeautifulSoup to collect diverse property data across Bangalore's regions. The collected data is saved in an Excel file for further processing.  
- **Data Analysis:** Cleaning and exploring Bangalore house rental data to handle missing values and outliers.  
- **Feature Engineering:** Transforming variables (like parsing area and extracting key amenities) to enhance model performance.  
- **Feature Selection:** Identifying the most significant features using:  
  - `rf_importance` (Random Forest Importance)  
  - `gb_importance` (Gradient Boosting Importance)  
  - `permutation_importance` (Permutation Importance)  
  - `rfe_score` (Recursive Feature Elimination Score)  
  - `SHAP_score` (SHAP Values for model explainability)  
- **Modeling:**  
  - Preprocessing with a `ColumnTransformer` to scale numeric features, apply ordinal encoding to categorical data, and one-hot encode regions.  
  - Implemented a Random Forest Regressor with parameters like `max_depth=20`, `max_features='sqrt'`, and `n_estimators=300`.  
  - Achieved an R² score of **0.93** on the test set, indicating strong model performance.  
- **Evaluation:** Analyzing model accuracy, with additional validation using the scraped data, achieving an R² score of **0.87**, confirming the model's robustness.  
- **Deployment:** The model is deployed using Streamlit, providing an interactive web application for users to predict house rents based on input features.  

### 🚀 Technologies Used  
- Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, BeautifulSoup/Selenium for scraping)  
- Jupyter Notebook  
- Machine Learning Algorithms (Linear Regression, Random Forest, etc.)  
- Streamlit for deployment  

### 🔗 Live Demo  
Check out the live application here: [Bangalore House Rent Predictor](https://bangalore-house-rent-predictor.streamlit.app/)

# Car Price Prediction with Machine Learning 🚗💰

![Car Price Prediction Banner](https://images.unsplash.com/photo-1550355291-bbee04a92027?ixlib=rb-4.0.3&auto=format&fit=crop&w=1000&q=80)

This repository contains my third task for the **CodeAlpha Data Science Internship**: Car Price Prediction using Machine Learning.

## 📌 Project Overview
The used car market is vast and dynamic. Determining the fair price of a used car can be challenging due to various influencing factors like brand goodwill, mileage, age, and fuel type. This project aims to build a robust Machine Learning regression model to accurately predict the selling price of a used car based on these features.

## 💾 Dataset
The dataset used in this project is sourced from Kaggle:
**[Car Price Prediction (Used Cars)](https://www.kaggle.com/datasets/vijayaadithyanvg/car-price-predictionused-cars)**

*Note: To run the notebook locally, please download the `car data.csv` file from Kaggle and place it in this repository's root directory.*

## 🛠️ Technologies Used
- **Python 3.x**
- **Pandas & NumPy** (Data Processing & Feature Engineering)
- **Matplotlib & Seaborn** (Data Visualization & EDA)
- **Scikit-Learn** (Label Encoding, Scaling, and Machine Learning)

## 📊 Methodology
1. **Data Preprocessing & Feature Engineering**: 
   - Derived a new feature, `Car_Age`, from the original `Year` column.
   - Dropped high-cardinality nominal columns (like `Car_Name`) to simplify the model.
   - Applied Label Encoding to categorical variables (`Fuel_Type`, `Seller_Type`, `Transmission`).
2. **Exploratory Data Analysis (EDA)**:
   - Visualized the distribution of the target variable (`Selling_Price`).
   - Generated a correlation heatmap to understand the relationships between numerical features. `Present_Price` showed the strongest positive correlation with `Selling_Price`.
3. **Modeling**: 
   - Split the dataset into 80% training and 20% testing sets.
   - Standardized the features using `StandardScaler`.
   - Trained a `RandomForestRegressor`.
4. **Evaluation**:
   - Assessed model performance using R-squared (R²), Mean Absolute Error (MAE), and Mean Squared Error (MSE).
   - Plotted a scatter chart of Actual vs. Predicted values to visually verify accuracy.

## 📈 Results
The Random Forest Regressor demonstrated excellent predictive capabilities, achieving a high R² score. The scatter plot of the actual versus predicted prices showed a tight clustering along the diagonal, confirming the model's reliability in estimating used car prices.

## 🚀 How to Run
1. Clone this repository.
2. Download the dataset from the Kaggle link provided above and ensure the file is named `car data.csv`.
3. Install the required dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```
4. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Car_Price_Prediction.ipynb
   ```

---
**Author**: [Your Name/Azzya]  
**Internship**: CodeAlpha - Data Science Intern

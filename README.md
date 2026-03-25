🏠 House Price Prediction (Kaggle Advanced Regression)
This project is based on the Kaggle House Prices Advanced Regression competition, where the goal is to predict house sale prices using various features describing residential homes.

📌 Problem Statement
Predict the SalePrice of houses based on features like:
* Area
* Location-related attributes
* Year built
* Number of rooms
* Quality indicators

📊 Dataset
Source: Kaggle
Dataset contains:
* Numerical features (area, year, etc.)
* Categorical features (neighborhood, condition, etc.)
* Missing values and skewed distributions

⚙️ Project Workflow
1. Exploratory Data Analysis (EDA)
* Identified missing values
* Analyzed relationship between features and target (SalePrice)
* Classified features into:
* Numerical
* Categorical
* Temporal

2. Feature Engineering
✔ Handling Missing Values:
* Categorical → replaced with "Missing"
* Numerical → filled with median
* Created indicator variables for missing data

✔ Temporal Features:
* Converted years into age-based features

✔ Skewness Handling:
* Applied log transformation to:
* Continuous variables
* Target (SalePrice)

✔ Rare Category Handling:
* Grouped categories with <1% frequency into "Rare"

✔ Encoding:
* Applied One-Hot Encoding

3. Data Preprocessing
* Removed unnecessary columns (Id)
* Created training features (X) and target (y)

📈 Key Insights
* Many features had missing values but still strong predictive power
* Data was highly skewed, requiring transformation
* Temporal variables significantly influenced house prices
* Rare categories can introduce noise → handled carefully

🚀 Future Improvements
* Add machine learning models (Linear Regression, XGBoost, etc.)
* Perform hyperparameter tuning
* Use cross-validation
* Feature selection techniques

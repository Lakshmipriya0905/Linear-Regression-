🏠 Housing Price Prediction using Linear Regression

This project demonstrates how to build a Linear Regression model to predict house prices based on various features like area, number of bedrooms, location info, and more using Python and Scikit-Learn in Google Colab.


---

📁 Dataset

File name: Housing.csv.xlsx

Contains features like:

area, bedrooms, bathrooms, stories, etc.

Categorical columns: mainroad, guestroom, furnishingstatus, etc.

Target variable: price




---

🔧 Steps Followed

1. Import Libraries

pandas, numpy, matplotlib, seaborn, sklearn



2. Load Data

Uploaded using files.upload() and read using pd.read_excel()



3. Preprocess Data

Removed missing values with df.dropna()

Converted categorical variables with pd.get_dummies()



4. Split Features and Target

X = df.drop('price', axis=1)

y = df['price']



5. Train-Test Split

Used train_test_split() from sklearn (80% train / 20% test)



6. Model Training

Linear Regression using LinearRegression().fit()



7. Evaluation

Metrics used: MAE, MSE, R²



8. Interpretation

Extracted coefficients and intercept



9. Visualization

Plotted actual vs predicted prices (based on area)

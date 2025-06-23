@@ -1 +1,54 @@
# task1
Task 1: Data Cleaning & Preprocessing

This project is part of the AI & ML Internship, focused on understanding how to clean and prepare raw data for machine learning.

Objective
The main goal is to:
- Handle missing values
- Encode categorical variables
- Scale numerical features
- Detect and remove outliers

Dataset
We used a dataset named `train_and_test2.csv`, which contains information related to passengers including:
- Age
- Fare
- Sex
- SibSp (Siblings/Spouses aboard)
- Pclass (Passenger class)
- Embarked
- 2urvived (Target variable)

Steps Followed

1. Import Libraries
Used libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`.

2. Load Dataset
Read the CSV file using `pandas`.

3. Explore Basic Info
- Checked null values and data types using `.info()` and `.isnull().sum()`.

4. Handle Missing Values
- Used **mean** for numerical columns like `Age` and `Fare`.
- Used **mode** for categorical columns like `Embarked`.

5. Encode Categorical Features
- Converted `Sex` to binary (`male=0`, `female=1`).
- One-hot encoded `Embarked`.

6. Normalize/Standardize Numerical Features
- Scaled `Age` and `Fare` using `StandardScaler` from `sklearn`.

7. Visualize and Remove Outliers
- Plotted boxplots.
- Used IQR (Interquartile Range) method to filter out extreme values.

Libraries Used

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `sklearn.preprocessing.StandardScaler`

# Property Price Prediction using PySpark Linear Regression

This project performs **multiple linear regression** on a property dataset using **PySpark** to predict house prices. It evaluates all combinations of 4 features from the available dataset and compares model performance using **R² Score**, **MSE**, and **RMSE**.

> Designed as a portfolio component and viva contribution for academic evaluation.

---

##  Project Overview

- **Dataset**: Real estate property data (loaded from CSV)
- **Goal**: Predict the `Price` using combinations of features
- **Models Used**:
  - Linear Regression
  - Automated comparison of multiple feature sets
- **Platform**: Google Colab + PySpark

---

##  Features Tested

From the dataset, the following features were used:

- `Square_Footage`
- `Num_Bedrooms`
- `Num_Bathrooms`
- `Year_Built`
- `Lot_Size`

The model evaluates every **4-feature combination** from the 5 available.

---

##  What the Notebook Does

1. Loads and preprocesses the property dataset
2. Splits the data into **training and testing sets**
3. Automates the training of **multiple linear regression models**
4. Prints results after each model: 
   - `Train R²`
   - `Test R²`
   - `MSE`
   - `RMSE`
5. Displays final sorted comparison table
6. Visualizes:
   - Top models by Test R²
   - MSE vs Test R² tradeoffs
   - Grouped metric comparison
   - Overfitting analysis (Train vs Test R²)

---

##  Example Outputs

| Features                                      | Train R² | Test R² | MSE (Test) | RMSE (Test) |
|----------------------------------------------|----------|---------|------------|-------------|
| Square_Footage, Num_Bedrooms, ..., Lot_Size  | 0.86     | 0.81    | 213000.55  | 461.56      |
| Square_Footage, Num_Bathrooms, ..., Year_Built | 0.84     | 0.79    | 228450.67  | 478.01      |

 Visualizations:
- Bar Chart: Top 5 combinations
- Scatter Plot: Overfitting detection
- Line and grouped bar plots

---

## 🛠 How to Run

1. Open [`Portfolio_1_Updated.ipynb`](./Portfolio_1_Updated.ipynb) in **Google Colab**
2. Mount your **Google Drive** if necessary
3. Upload your dataset as `property.csv` or update the path
4. Run each cell sequentially to view results and visualizations

---

## Repository Structure


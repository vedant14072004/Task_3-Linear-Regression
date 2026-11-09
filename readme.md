# Task 3: Linear Regression

## Objective
Implement and understand simple and multiple linear regression to predict house prices.

## Dataset
House Price Prediction dataset (Housing.csv) with features such as area, bedrooms, bathrooms, stories, parking, and yes/no amenities. The target is `price`.

## Steps Performed
1. **Preprocessing:** checked for missing values, converted yes/no columns to 1/0, and one-hot encoded `furnishingstatus`.
2. **Train-test split:** 80% training and 20% testing (`random_state=42`).
3. **Model fitting:** trained a simple linear regression (area only) and a multiple linear regression (all features) using scikit-learn.
4. **Evaluation:** measured MAE, MSE, RMSE and R² on the test set.
5. **Visualization and interpretation:** plotted the regression line and actual vs predicted prices, and interpreted the coefficients.

## Results
| Model | MAE | RMSE | R² |
|-------|-----|------|-----|
| Simple (area only) | ____ | ____ | ____ |
| Multiple (all features) | 970,043 | 1,324,507 | 0.653 |

## Key Findings
- Using all features gives better predictions than area alone.
- The multiple regression model explains about 65% of the variance in house prices.
- Each extra unit of area increases the predicted price by about ____, holding other features constant.
- The strongest positive features are ____ and ____.
- The two furnishing columns are correlated (-0.59) because they come from the same category. No other pair is strongly correlated.

## Tools Used
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

## Files
- `linear_regression.ipynb`: notebook with all steps
- `Housing.csv`: dataset
- `Screenshots/`: key outputs and plots
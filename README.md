# AI_Assignments

## Project Name
Linear Regression on Sport Car Prices Dataset

## Dataset Used
- Dataset Name: Sport Car Price Dataset
- Source: Kaggle
- Description: Contains car information such as Car Make, Car Model, Horsepower, Torque, 0-60 MPH Time, and Price in USD.

## Preprocessing Steps
1. Checked for missing values and filled them with mean values.
2. Dropped non-numeric columns like `Car Model` and `Engine Size (L)` (Electric cars had text values in Engine Size).
3. Converted numeric-looking columns (`Horsepower`, `Torque`, `0-60 MPH Time`) from strings to numbers.
4. Encoded categorical column `Car Make` using one-hot encoding.
5. Final dataset contains only numeric features and the target column `Price (in USD)`.

## Model Explanation
- We used **Linear Regression** to predict the price of a car based on its features.
- Linear Regression predicts continuous numerical values using a linear combination of features.
- Features used: Horsepower, Torque, 0-60 MPH Time, and encoded Car Make columns.

## Model Training
- Dataset split: 80% training, 20% testing.
- Model trained on `X_train` and `y_train`.
- Predictions made on `X_test`.

## Evaluation Metrics
- Mean Absolute Error (MAE): 116,221.80
- Mean Squared Error (MSE): 106,583,300,634.42
- R² Score: 0.8243

## Instructions to Run
1. Open the Colab notebook (`.ipynb`) in Google Colab.
2. Upload the dataset file `Sport car price.csv` to Colab.
3. Run all cells in order.
4. Check the outputs: dataset info, predictions, and evaluation metrics.

---

*This project was completed as part of the AI course assignments. All steps are explained in the notebook.*


## Project Name
Linear Regression on Sport Car Prices Dataset

## Student Email
syedintisarshahjaffary@gmail.com

## Dataset Used
- Dataset Name: Sport Car Price Dataset
- Source: Kaggle
- Description: Contains car information such as Car Make, Car Model, Horsepower, Torque, 0-60 MPH Time, and Price in USD.  
- Number of rows/columns: Check in Colab with `df.info()`  
- Target variable: `Price (in USD)`  
- Features used: Horsepower, Torque, 0-60 MPH Time, Car Make (encoded)

## Preprocessing Steps
1. Checked for missing values and filled them with the mean values of each column.
2. Dropped non-numeric columns (`Car Model` and `Engine Size (L)`), because Engine Size had text like 'Electric'.
3. Converted numeric-like columns (`Horsepower`, `Torque`, `0-60 MPH Time`) from strings to float.
4. Encoded categorical column `Car Make` using one-hot encoding.
5. Final dataset contains only numeric features ready for Linear Regression.

## Model Explanation
- We used **Linear Regression** to predict car prices.  
- Linear Regression predicts continuous numerical values from input features.  
- Features used in the model: Horsepower, Torque, 0-60 MPH Time, and encoded Car Make columns.  
- Target variable: Price in USD.

## Model Training
- Dataset split: 80% training, 20% testing (`train_test_split` in Python).  
- Model trained on `X_train` and `y_train`.  
- Predictions made on `X_test`.

## Evaluation Metrics
- **Mean Absolute Error (MAE):** 116,221.80  
- **Mean Squared Error (MSE):** 106,583,300,634.42  
- **R² Score:** 0.8243  

## Actual vs Predicted Prices
- The first 20 predictions vs actual prices are shown in the notebook (`comparison.head(20)`).  
- Optional: Pseudo confusion matrix based on price ranges is included to compare ranges visually.

## Instructions to Run
1. Open the Colab notebook (`.ipynb`) in Google Colab.  
2. Upload the dataset file `Sport car price.csv` to Colab.  
3. Run all cells in order.  
4. Check outputs:
   - Dataset info
   - Preprocessing steps
   - Linear Regression predictions
   - Actual vs Predicted table
   - Evaluation metrics (MAE, MSE, R²)
   - Optional: Pseudo confusion matrix for price ranges

---

*This project was completed as part of the AI course . All steps, preprocessing, model training, predictions, and evaluation metrics are explained in the notebook.*

# Dimensionality Reduction & Stock Price Prediction

This repository contains a **two-part project** in Python using Google Colab:  

1. **Dimensionality Reduction** – Reducing high-dimensional datasets to 2D using **Principal Component Analysis (PCA)**.  
2. **Stock Price Prediction** – Forecasting future stock prices using **ARIMA (AutoRegressive Integrated Moving Average)**.

## **Part 1: Dimensionality Reduction (PCA)**

### Objective
Reduce high-dimensional data (Iris dataset) to **two dimensions** for visualization.

### Steps
1. Load the Iris dataset from `sklearn.datasets`.
2. Apply PCA to reduce dimensions from 4 to 2.
3. Visualize the reduced data using a scatter plot.

### Deliverables
- 2D reduced dataset.
- Scatter plot of the 2D representation.

### Sample Visualization
![PCA Scatter Plot](images/pca_scatter.png)  

## **Part 2: Stock Price Prediction (ARIMA)**

### Objective
Predict future stock prices based on historical data.

### Dataset
- File: `stock_prices.csv`  
- Columns: `Date`, `Open`, `Close`, `Volume`  
- Sample data: [Apple Stock Prices CSV](https://raw.githubusercontent.com/plotly/datasets/master/finance-charts-apple.csv)

### Steps
1. Load and preprocess dataset
   - Convert `Date` to datetime
   - Set `Date` as index
   - Handle missing values with interpolation
2. Exploratory Data Analysis (EDA)
   - Plot `Close` price trend
3. Train-Test Split
   - Use last 100 days as test set
4. Train ARIMA Model
   - Fit ARIMA using `statsmodels`
   - Forecast next 100 days
5. Evaluate Model
   - Metrics: MAE, RMSE, MAPE
6. Visualize Forecast vs Actual Prices

### Sample Plot
![ARIMA Forecast](images/arima_forecast.png)  

## **How to Run**

1. Open [Google Colab](https://colab.research.google.com/).  
2. Copy the Python code from the notebooks or this repository.  
3. Run **Part 1** to see PCA results.  
4. Run **Part 2** to forecast stock prices.
## **Requirements**
- Python 3.x  
- Libraries:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `scikit-learn`
  - `statsmodels`
  - `sklearn`  

Install dependencies using:

```bash
pip install pandas numpy matplotlib scikit-learn statsmodels

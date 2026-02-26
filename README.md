# Weather-Prediction-using-Machine-Learning-Python
# Weather Temperature Prediction 

This project explores the relationship between weather variables using a historical weather dataset. It specifically focuses on predicting **Temperature** based on **Wind Speed** using Linear Regression.

## Dataset Overview
The dataset (`weatherHistory.csv`) contains approximately 96,453 records with features such as:
* **Temperature (C)** (Target)
* **Wind Speed (km/h)** (Predictor)
* Humidity, Pressure, and Visibility
* Precipitation Type and Summary

## Implementation
The analysis is performed in a Jupyter Notebook (`weather.ipynb`) using the following stack:
- **Pandas & NumPy**: For data cleaning and manipulation.
- **Matplotlib**: For visualizing the correlation and regression line.
- **Scikit-Learn**: For building the `LinearRegression` model and preprocessing.

### Key Steps:
1. **Data Cleaning**: Handled missing values in the `Precip Type` column.
2. **Exploratory Data Analysis (EDA)**: Visualized the distribution of wind speed vs. temperature.
3. **Modeling**: Built an Ordinary Least Squares (OLS) regression model.
4. **Feature Scaling**: Evaluated the impact of `StandardScaler` on model performance and interpretability.

## Results
The model demonstrates the trend between wind velocity and ambient temperature. While feature scaling (Z-score normalization) does not alter the predictive power ($R^2$) of this specific linear model, it provides a foundation for more complex algorithms like Gradient Descent or Support Vector Machines.

### Visualizations
The notebook includes:
- **Scatter Plot**: Raw data distribution.
- **Regression Line**: The "Best Fit" line plotted against actual values.

## Run the notebook:
    jupyter notebook weather.ipynb
  
## Install dependencies:
   ```bash
pip install pandas scikit-learn matplotlib

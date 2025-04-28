# Car Price Prediction — Multiple Linear Regression

This project builds a **multiple linear regression model** to predict car prices based on various vehicle features. It uses a Kaggle dataset and includes data preprocessing, feature selection, visualization, model training, and evaluation.

## Dataset

- **Source**: [Kaggle - Car Price Prediction](https://www.kaggle.com/datasets/hellbuoy/car-price-prediction)
- **Description**: The dataset contains information on different car characteristics (e.g., horsepower, curb weight, engine size, etc.) and their corresponding market prices.
- **Size**: 26 columns, 205 rows.

Key columns:
- `symboling`, `wheelbase`, `curbweight`, `horsepower`, `cylindernumber`, and more.
- `price` (target variable).

Some columns like `car_ID`, `CarName`, and `fuelsystem` were dropped as they are not useful for prediction.

## Methodology

1. **Data Loading and Cleaning**  
   - Downloaded using `kagglehub`.
   - Dropped irrelevant columns.
   
2. **Exploratory Data Analysis (EDA)**  
   - Scatter plots were created for features like horsepower, curb weight, and wheelbase against price to visualize relationships.

3. **Feature Engineering**  
   - Standardized the features using `StandardScaler`.
   
4. **Model Building**  
   - Applied **Multiple Linear Regression**.
   - Split the data into training and testing sets (90% training, 10% testing).

5. **Model Evaluation**  
   - Used **Root Mean Squared Error (RMSE)** to assess performance.

## Results

- The regression model achieved decent performance on predicting car prices.
- Visualized predictions vs actual prices using scatter plots.

## How to Run

1. Clone this repository:

    ```bash
    git clone https://github.com/yourusername/car-price-prediction.git
    cd car-price-prediction
    ```

2. Install required packages:

    ```bash
    pip install pandas numpy matplotlib scikit-learn kagglehub
    ```

3. Run the Jupyter Notebook:

    ```bash
    jupyter notebook car_price_prediction.ipynb
    ```

**Note:** You need Kaggle API credentials set up to download datasets via `kagglehub`.

## Requirements

- Python 3.8+
- pandas
- numpy
- matplotlib
- scikit-learn
- kagglehub


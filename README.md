# Real Estate Sales Analysis and Price Prediction (2001-2022)

This project performs an **Exploratory Data Analysis (EDA)** and builds an initial **predictive model** for real estate sale prices based on a dataset of property transactions from 2001 to 2022.

The goal is to explore the data, understand key factors affecting property prices, and build a simple predictive model to estimate sale prices.


## Dataset

- **Source:** [Real Estate Sales 2001-2022 on Kaggle](https://www.kaggle.com/datasets/omniamahmoudsaeed/real-estate-sales-2001-2022)  
- **File:** `real-estate-sales-2001-2022.csv`


## Tools Used

- **Programming Language:** Python
- **Libraries:**
  - Pandas
  - Numpy
  - Matplotlib
  - Seaborn
  - Scikit-learn


## Project Structure

1. **Exploratory Data Analysis (EDA)**
    - Data Cleaning:
        - Removing missing values (`NaN`)
        - Handling duplicates
        - Standardizing date formats
    - Feature Exploration:
        - Town, property type, residential type, floor area
    - Temporal Analysis:
        - Price trends over time (by Date of Sale)
    - Outlier Detection:
        - Identifying extreme values in Price and Floor Area
    - Correlation Check:
        - Exploring relationships between numerical features

2. **Predictive Modeling**
    - Model used: **Linear Regression**
    - Train-test split performed
    - Model evaluated using:
        - R² score
        - Root Mean Squared Error (RMSE)


## Results

### Model Performance:

- **Test R² score:** 0.2854
- **Test RMSE:** 627,731.69

### Interpretation:

- The **R² score of 0.2854** indicates that the model explains approximately 28.5% of the variance in sale prices.
- The **RMSE of ~627K** suggests that predictions have a high average error — this is expected given that a simple Linear Regression model was used.


## Conclusion

- The EDA successfully identified several key factors affecting property prices, such as:
    - Location (town and region)
    - Property type and residential type
    - Floor area
    - Temporal trends in sale prices
- The initial model (Linear Regression) provided a basic understanding of price prediction, but performance is limited and can be improved with more advanced models.


## Recommendations for Next Steps

1. **Feature Engineering**
    - Create new features (e.g., `price per sqm`, `year of sale`) to extract more value from the data.
2. **Model Development**
    - Explore more complex models such as Random Forest or Gradient Boosting to improve prediction accuracy.
3. **Data Imputation**
    - Handle missing values systematically using appropriate imputation methods.
4. **Outlier Treatment**
    - Address extreme values to reduce noise in the model.
5. **Advanced Exploration**
    - Investigate interaction effects and potential clustering for deeper insights.


## License

For educational purposes only.

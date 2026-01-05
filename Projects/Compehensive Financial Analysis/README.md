# Leveraging Machine Learning for Financial & Predictive Stock Analysis

## Overview

This project applies statistical analysis and machine learning techniques to analyze financial performance and predict stock price movements for a set of listed companies. It combines exploratory data analysis, linear and non-linear modeling, and predictive ranking to identify key financial drivers of stock performance and generate actionable insights for investment decision-making.

Users are encouraged to explore the code, review the report, and adapt the workflow to their own datasets or investment strategies.

---

## Dataset Description

The analysis uses a comprehensive financial dataset obtained from  [**kaggle**](https://www.kaggle.com/datasets/pacificrm/financial-sheets), containing time-series financial and market data for multiple companies.

### Data Includes:

- **Financial Statements:** Annual and quarterly profit & loss, balance sheet, and cash flow data  
- **Market Data:** Stock prices and market capitalization  
- **Financial Ratios:** Profitability, leverage, efficiency, and growth metrics  
- **Time Dimension:** Financials at T0 and corresponding market prices at T1  

### Dataset Structure:

- **Observations:** ~3,000 company-quarter records  
- **Features:** 9 key financial and operational indicators  
- **Target Variable:** `price_change_%` (quarterly percentage change in stock price)  
- **Additional Metadata:** Company name and reporting date  

### Key Features Used:

- Return on Capital Employed (ROCE, capped for outliers)  
- Operating Profit Margin (OPM)  
- Asset Turnover (ATO)  
- Return on Assets (ROA)  
- Debt-to-Equity Ratio  
- EPS Growth (3 Years)  
- PEG Ratio  
- Market Capitalization  
- Composite Efficiency Score  

> Ensure the dataset is correctly placed and referenced in the code before execution.

---

## Machine Learning Approach

### Algorithms Used:

- Linear Regression (OLS)  
- Ridge, Lasso, and Elastic Net Regression  
- Random Forest Regressor  
- Gradient Boosting Regression  
- XGBoost  
- Multi-Layer Perceptron (MLP) Neural Network  

### Evaluation Metrics:

- R-squared (R²)  
- Root Mean Squared Error (RMSE)  
- Mean Absolute Error (MAE)  

> Cross-validation and hyperparameter tuning were performed using `GridSearchCV`.

---

## Setup and Usage

### Prerequisites

- Python 3.x  
- Required libraries:  
  `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `xgboost`  

### Steps

1. **Clone this Repository**

```bash
git clone https://github.com/Isadare-Oreoluwa/ml-projects.git
cd ml-projects
````

2. **Install Dependencies**

```bash
pip install pandas numpy scikit-learn matplotlib seaborn xgboost
```

3. **Adjust File Locations**

* Open the analysis scripts.
* Locate where the CSV file is referenced.
* Update the file path to your local dataset location.

Example:

```python
data = pd.read_csv('data/financial_data.csv')
```

4. **Run the Scripts**

Execute the analysis scripts to:

* Perform exploratory data analysis (EDA)
* Train the machine learning models
* Generate predictions

---

## Results and Insights

### Best Performing Model

**Random Forest Regressor**

* R-squared: ~0.23
* RMSE: ~6.05

### Key Drivers of Stock Price Changes

* Market Capitalization
* Return on Capital Employed (ROCE)
* Return on Assets (ROA)
* Debt-to-Equity Ratio

### Key Findings

* Linear models show limited predictive power, indicating weak linear relationships between financial metrics and short-term price movements.
* Tree-based models capture non-linear interactions and provide more reliable predictions.
* Profitability metrics are strongly interrelated, while leverage and liquidity indicators exhibit weaker linear correlations.

### Predictive Output

* The model generates a ranked list of stocks with the highest predicted quarterly price increases using the latest available data.

---

## Notes

* This project emphasizes **methodological rigor**, including outlier treatment, feature engineering, scaling decisions, and residual diagnostics.
* The code is designed as a flexible framework; users can expand it with macroeconomic variables or time-series models.
* Results should be interpreted as **decision-support tools**, not financial advice.

---



## References
- *Report:* [Detailed Report](https://github.com/Isadare-Oreoluwa/ML-projects/blob/ML-main/Projects/Compehensive%20Financial%20Analysis/Comprehensive%20Financial%20Analysis%20Report.pdf)
- *Code & Data:* [Available in this repository](https://github.com/Isadare-Oreoluwa/ML-projects/tree/ML-main/Projects/Compehensive%20Financial%20Analysis/Data%20and%20Code)



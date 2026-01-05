# Leveraging Machine Learning for Predicting Agricultural Trade Flows

## Overview
This project demonstrates the application of machine learning techniques to predict agricultural trade flows between Nigeria and its trading partners. It identifies key factors influencing trade and evaluates the performance of various algorithms in predicting trade patterns. Users are encouraged to explore the code and customize it to suit their data and file paths.

## Dataset Description
The analysis uses a CSV file containing trade-related data, including:  
- **Trade Metrics:** Import and export values in USD.  
- **Economic Indicators:** GDP and exchange rates.  
- **Demographics:** Population data for Nigeria and its trading partners.  
- **Geographical Factors:** Distance, landlocked status, and shared languages.

Ensure the CSV file is correctly placed and referenced in the code for successful execution.

## Machine Learning Approach
### Algorithms Used:
- Linear Regression (including Ridge and Lasso variants)  
- Random Forest  
- Gradient Boost Regression  
- Neural Networks  

### Evaluation Metrics:
- R-squared (R²)  
- Mean Squared Error (MSE)  
- Root Mean Squared Error (RMSE)  

## Setup and Usage
### Prerequisites:
- Python 3.x installed on your system.  
- Required libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`.  

### Steps:
1. **Clone this Repository:**  
   Download the project files, including the scripts and CSV data.  
   ```bash
   git clone https://github.com/Isadare-Oreoluwa/ml-projects.git
   cd ml-projects
   ```

2. **Install Dependencies:**  
   Manually install the required libraries:  
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```

3. **Adjust File Locations:**  
   - Open the analysis and visualization scripts in a text editor.  
   - Locate where the CSV file is referenced.  
   - Update the file path to match the location of your dataset.  

   Example:  
   If your dataset is stored in `C:/datasets/trade_data.csv`, change:  
   ```python
   data = pd.read_csv('data/trade_data.csv')
   ```
   To:  
   ```python
   data = pd.read_csv('C:/datasets/trade_data.csv')
   ```

4. **Run the Scripts:**  
   Execute the analysis script to process the data and generate results:  

## Results and Insights
- **Best Model for Imports:** Random Forest  
  - R-squared: 0.75  
  - MSE: 3.60699E+15
- **Key Factors Influencing Trade:**  
  - GDP and population of trading partners.  
  - Exchange rates and distance.  


## Notes
- The code is provided as a starting point; users should edit paths to fit their local environment.
- For any issues or questions, feel free to raise an issue in this repository or reach out via email.

## References
- *Report:* [Detailed Report](https://github.com/Isadare-Oreoluwa/ML-projects/blob/ML-main/Projects/Predicting%20Agricultural%20trade%20flow%20between%20Nigeria%20and%20her%20trading%20partners/Agricultural%20Trade%20Flows%20Prediction%20report.docx)  
- *Code and Data:* [Download Files](https://github.com/Isadare-Oreoluwa/ML-projects/tree/ML-main/Projects/Predicting%20Agricultural%20trade%20flow%20between%20Nigeria%20and%20her%20trading%20partners/Data%20and%20Code) 

# Customer Churn Prediction - Telco

## Project Overview

Retaining customers is crucial for a company's success, particularly in the highly competitive wireless services industry. Acquiring new customers is not only more challenging but also significantly more costly than maintaining existing customer relationships. This project focuses on predicting customer behavior to help Telco, a home phone and internet service provider, retain its customers and reduce churn.

The primary objective is to develop a predictive model that identifies key factors influencing customer attrition, allowing Telco to proactively address churn risks and enhance its customer retention strategies.

## Data Overview

The dataset used in this analysis consists of 7,043 records with 20 attributes, which can be categorized into two main groups:

- **Customer Demographic Data:** Includes features such as gender, marital status (partnered or not), presence of dependents, and whether the customer is 65 years or older.
  
- **Account Information:** Covers details such as the length of time a customer has been with Telco, their monthly and total charges, the type of contract (month-to-month, one-year, or two-year), and the types of services (phone, internet, TV) they subscribe to.

The target variable for this study is **Churn**, a binary indicator that shows whether or not a customer left within the last month.

### Data Preprocessing

- **Missing Values:** There were 11 records with missing values in the `TotalCharges` feature. Given the small number of missing observations, these records were removed, resulting in a final dataset of 7,032 customers.

- **Categorical Variables:** Several Yes/No categorical variables contained an additional group indicating that the customer had no phone or internet service. These were recoded and combined with the `No` category for consistency.

## Methodology

1. **Exploratory Data Analysis (EDA):**  
   The project begins with an exploratory analysis to understand the relationships between the features and the target variable, Churn. EDA helps identify which factors are most influential in predicting customer attrition.

2. **Feature Engineering:**  
   Based on the EDA, new features were created or transformed to improve the predictive power of the model.

3. **Model Development:**  
   Several machine learning models were developed and evaluated to predict customer churn. The models were assessed based on their accuracy, precision, recall, and other relevant metrics.

4. **Model Interpretation and Insights:**  
   The most effective model was analyzed to understand which features were most significant in predicting churn. These insights were used to recommend strategies for reducing customer attrition.

## Results

The analysis identified several key factors that contribute to customer churn at Telco, including:

- **Contract Type:** Customers with month-to-month contracts were more likely to churn compared to those with longer contracts.
- **Tenure:** Longer tenure was associated with lower churn rates.
- **Monthly Charges:** Higher monthly charges correlated with a higher likelihood of churn.

## Conclusion

This project demonstrates the importance of understanding customer behavior in the wireless services industry. By leveraging predictive modeling and data analysis, Telco can reduce its churn rate, improve customer retention, and ultimately enhance its competitive position in the market.

## Files Included

- `data/`: Contains the cleaned Telco customer dataset.
- `results/`: Outputs and visualizations generated from the analysis.
- `Rmd/`: R Markdown files documenting the entire analysis process.
- `presentation/`: A summary presentation of the project findings.
- `README.md`: This document.

## How to Run

1. Clone the repository.
2. Install the required R packages listed in the `Rmd/` files.
3. Open the R Markdown files in the `Rmd/` directory and run the analysis to reproduce the results.

## Acknowledgments

This project was conducted as part of a predictive analytics study, focusing on customer retention strategies in the telecommunications industry.

# Loan Repayment Prediction Using Ensemble Learning Methods

This project aims to predict whether a bank should approve a loan application based on the applicant's financial profile, utilizing various Ensemble Learning methods.

## Objective

Predict loan repayment status based on applicant data.

## Dataset

The dataset used in this project is `loan_data.csv`. It contains various features related to loan applicants, including:

- `credit.policy`: 1 if the customer meets the credit underwriting criteria, 0 otherwise.
- `purpose`: The purpose of the loan (e.g., debt_consolidation, credit_card, etc.).
- `int.rate`: The interest rate of the loan.
- `installment`: The monthly installments owed by the borrower.
- `log.annual.inc`: The natural log of the borrower's annual income.
- `dti`: The debt-to-income ratio of the borrower.
- `fico`: The FICO credit score of the borrower.
- `days.with.cr.line`: The number of days the borrower has had a credit line.
- `revol.bal`: The borrower's revolving balance (amount unpaid at the end of the billing cycle).
- `revol.util`: The borrower's revolving line utilization rate (the amount of the credit line used relative to total credit available).
- `inq.last.6mths`: The number of inquiries by creditors in the last 6 months.
- `delinq.2yrs`: The number of times the borrower has been 30+ days past due on a payment in the past 2 years.
- `pub.rec`: The number of derogatory public records (bankruptcy filings, tax liens, judgments).
- `not.fully.paid`: 1 if the loan was not fully paid, 0 otherwise (this is the target variable).

## Methodology

1.  **Data Loading and Exploration**: Load the dataset and perform initial data exploration to understand the structure, data types, and identify missing values.
2.  **Data Preprocessing**: Handle categorical features (`purpose` attribute) using Label Encoding.
3.  **Data Visualization**: Visualize key relationships and distributions within the data, such as the relationship between FICO scores, interest rates, and loan repayment status.
4.  **Train-Test Split**: Split the dataset into training and testing sets to evaluate model performance.
5.  **Model Training and Evaluation**: Train and evaluate various ensemble learning models, including:
    - Decision Tree
    - Bagging with Decision Tree
    - AdaBoosting with Decision Tree
    - Random Forest Classifier
    - AdaBoosting with Random Forest
    - Gradient Boosting

## Results

The performance of each model is evaluated based on accuracy, precision, recall, and confusion matrix. The notebook provides a comparison of the results obtained from different ensemble methods.

*(You can add a summary of the best performing model and its metrics here after running all the cells)*

## How to Run the Notebook

1. Clone the repository to your local machine.
2. Make sure you have Python and the necessary libraries installed (e.g., pandas, numpy, matplotlib, seaborn, scikit-learn).
3. Open the notebook in a Jupyter environment (like Google Colab or Jupyter Notebook).
4. Run the cells sequentially.

## Dependencies

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

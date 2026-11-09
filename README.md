# Credit Card Worthiness Prediction Model

## Project Overview
The Credit Card Worthiness Prediction Model is a machine learning project that evaluates an individual's financial information and predicts their creditworthiness.

The project uses classification algorithms to learn patterns from an existing financial dataset and predict whether a new applicant belongs to the good or poor creditworthiness category.

**Note:** The available dataset contains loan approval records. Therefore, this project uses historical loan approval as a proxy for creditworthiness. It does not directly predict credit card repayment or default risk.

## Objectives
- Analyze financial information to identify patterns related to creditworthiness.
- Train and compare multiple machine learning classification models.
- Evaluate model performance using standard evaluation metrics.
- Accept new applicant details and generate predictions.

## Dataset
**File:** `loan_approval.csv`

The dataset contains the following attributes:

| Feature | Description |
|---|---|
| income | Applicant's income |
| credit_score | Applicant's credit score |
| loan_amount | Requested loan amount |
| years_employed | Number of years employed |
| points | Financial points recorded in the dataset |
| loan_approved | Historical loan approval status (target) |

The `name` and `city` columns are excluded from model training.

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Google Colab

## Machine Learning Algorithms
The project trains and compares the following classification algorithms:

1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier

The best-performing model is selected based on ROC-AUC score.

## Project Workflow
1. Upload the existing CSV dataset.
2. Load and preprocess the data.
3. Handle missing and invalid values.
4. Perform feature engineering by calculating the loan-to-income ratio.
5. Split the dataset into training and testing sets.
6. Train the classification models.
7. Evaluate model performance using:
   - Accuracy
   - Precision
   - Recall
   - F1-score
   - ROC-AUC
8. Select the best-performing model.
9. Accept new applicant details through user input.
10. Predict the applicant's creditworthiness.

## How to Run
1. Open [Google Colab](https://colab.research.google.com/).
2. Create a new notebook.
3. Copy the project Python code into a code cell.
4. Run the cell.
5. Upload the `loan_approval.csv` dataset when prompted.
6. Enter the applicant's financial details when requested.
7. View the predicted result.

## Expected Output
The model displays:
- Selected machine learning algorithm.
- Model evaluation metrics.
- Classification report and confusion matrix.
- Predicted creditworthiness: GOOD or POOR.
- Probability of historical loan approval.

## Future Enhancements
- Use a real credit card dataset containing repayment and default history.
- Include payment history, credit utilization, outstanding balance, and missed payments.
- Develop a web interface for user interaction.
- Improve prediction reliability through additional features and model tuning.

## Conclusion
This project demonstrates how machine learning classification algorithms can be used to analyze financial data and generate predictions for new applicants. It provides a basic prototype for creditworthiness assessment using historical loan approval data.
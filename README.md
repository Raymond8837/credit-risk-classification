# credit-risk-classification

## Overview of the Analysis
- Purpose of the analysis: The purpose of this analysis was to evaluate the credit risk of borrowers by predicting whether a loan is a high-risk or healthy (low-risk) loan. This was done using a logistic regression model based on financial data.


- Financial information: The dataset used in this analysis consists of information on loans, including the borrowers' loan amount, interest rates, and incomes. The target variable we aimed to predict was the loan_status, where 0 represents healthy loans and 1 represents high-risk loans.


- Variables: The variables used to predict loan risk included various financial indicators such as loan_amount, interest_rate, and income. We used the loan_status column as the label to predict the loan's risk.


- Stages of the machine learning process:

    - Data Preprocessing: The dataset was cleaned and split into training and testing sets.
    - Model Training: A logistic regression model was trained on the training set using loan_status       as the label.
    - Model Evaluation: The model was evaluated using the test set, and a classification report was       generated to assess its performance.

- Methods used: Logistic regression was selected as the classification model because it is suitable for binary classification problems like predicting credit risk. The train_test_split function was used to divide the data, and classification_report and confusion_matrix were used for performance evaluation.

## Results
Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

- Machine Learning Model 1 (Logistic Regression):
    - Accuracy: The logistic regression model achieved an accuracy of approximately 99% on the test       set.
    - Precision:
      - For class 0 (healthy loans): 100%
      - For class 1 (high-risk loans): 88%
    - Recall:
      - For class 0: 100%
      - For class 1: 91%
    - F1-score:
      - For class 0: 100
      - For class 1: 89
These scores indicate the model's ability to correctly classify both healthy and high-risk loans, with higher precision and recall scores for one class suggesting better model performance in that area.

## Summary
Summarise the results of the machine learning models, and include a recommendation on the model to use, if any.

    - Best Performing Model: The logistic regression model performed reasonably well, with an overall accuracy of 99% and strong precision and recall scores for predicting both classes. The F1-scores indicate balanced performance between precision and recall.

    - Important Considerations: If the primary goal is to avoid misclassifying high-risk loans (class 1), it is important to focus on the recall score for class 1, which measures the model's ability to correctly identify high-risk loans. Conversely, if avoiding false positives (incorrectly labeling healthy loans as high-risk) is more critical, we should focus on precision for class 1.

    - Recommendation: Based on the current results, the logistic regression model is recommended for identifying credit risk. However, further tuning may be required to improve the balance between precision and recall, particularly if the company's focus is on minimizing false negatives (failing to identify high-risk loans).
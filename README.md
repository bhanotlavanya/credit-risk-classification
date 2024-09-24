# credit-risk-classification
Project Objective:
The goal of this project was to analyze a historical dataset of loan applicants provided by a bank to develop a predictive model that can assess the creditworthiness of future borrowers. The bank aims to utilize this model to approve loans for applicants who are more likely to repay while minimizing approvals for those likely to default, thus reducing the risk of bad loans.

Dataset Overview:
The dataset consisted of 77,536 loan applicants and included the following features:

Loan amount
Interest rate on the loan
Borrower's income
Debt-to-income ratio
Number of accounts used by the borrower
Derogatory marks on the borrower's credit report
Borrower's total debt
Loan status: where '0' denotes a healthy loan applicant and '1' indicates an applicant who defaulted (considered high-risk).
After removing the loan status column, the data was split into a training set (75%) and a testing set (25%), reflecting the percentage of defaults in the dataset. A logistic regression model was trained on the training data and used to make predictions on the test set. The model's performance was evaluated using a confusion matrix and a classification report.

Model Performance:
Accuracy: Accuracy represents the percentage of correct predictions made by the model. The weighted accuracy of the logistic regression model was 99%, accounting for both precision and recall across all classes, with results averaged based on the number of samples per class. The macro accuracy (unweighted) was 92% for healthy loans and 95% for high-risk loans. Overall, the model achieved a 99% weighted accuracy, indicating excellent performance.

Precision: Precision measures how accurate the model is when predicting positive instances. In this case, the model achieved a 100% precision for healthy loan applicants (those who are less likely to default) and 85% precision for high-risk loan applicants. This suggests that the model performs well in identifying healthy loans, though the prediction accuracy for high-risk loans is lower but still within an acceptable range.

Recall: Recall measures the model’s ability to correctly identify positive instances. The recall score for healthy loan applicants was 99%, while for high-risk applicants, it was 91%. This indicates that the model is better at identifying healthy applicants compared to high-risk ones.

Summary:
The model works extremely well in case of prediction a low risk loan where as when it comes to predicting high risk loans it can be only trusted to 85% which is clear from the confusion matrix as well

The model predicted a total of 19,384 applicants, with the following outcomes:

18,663 true positives
56 false positives
102 false negatives
563 true negatives
Given the model's strong performance in predicting healthy loans and its reasonable accuracy in predicting high-risk applicants, I recommend the bank adopt this model. It should prove valuable in managing credit risk by minimizing loan defaults and approving loans for reliable applicants.
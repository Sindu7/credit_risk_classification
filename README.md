# credit_risk_classification

Overview of the Analysis:

Explain the purpose of the analysis.

    The purpose of this analysis is to harness machine learning techniques to forecast the risk associated with loans, using various financial indicators. This approach is crucial for financial organizations to evaluate the risk involved in loan applications.

Explain what financial information the data was on, and what you needed to predict.

    The dataset contains financial metrics such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The target variable is loan_status, where 1 indicates a high-risk loan and 0 indicates a low-risk loan.

Provide basic information about the variables you were trying to predict (e.g., value_counts).

    The dataset has a class imbalance, with 75,036 low-risk loans and 2,500 high-risk loans.

Describe the stages of the machine learning process you went through as part of this analysis. Briefly touch on any methods you used (e.g., LogisticRegression, or any resampling method).

    The process includes data preparation, dividing it into training and testing subsets, applying logistic regression models to both the original and adjusted (resampled) datasets, and assessing the outcomes using metrics like accuracy, precision, recall, and the F1-score.

Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

    Different methodologies, such as Logistic Regression and data resampling techniques, were employed in this analysis.

Results:

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

    Machine Learning Model 1: Logistic Regression Model with Original Data

        Balanced Accuracy: Approximately 95.2%.
        Confusion Matrix: True Negatives: 18,663, False Positives: 102, False Negatives: 56, True Positives: 563.
        Classification Report: For healthy loans, the precision, recall, and F1-score are all approximately 100%. For high-risk loans, precision is 85%, recall is 91%, and F1-score is 88%.

    Machine Learning Model 2: Logistic Regression Model with Resampled Data

        Balanced Accuracy: Approximately 99.45%.
        Confusion Matrix: True Negatives: 74,614, False Positives: 422, False Negatives: 403, True Positives: 74,633.
        Classification Report: The logistic regression model trained with oversampled data (where the number of high-risk and low-risk loans in the training set is equalized) is said to predict with near-perfect accuracy (99%).

Summary:
   
    The analysis revealed that both logistic regression models are highly effective in predicting loan risk.

    Model with Original Data: Exhibits excellent precision, recall, and F1-scores for low-risk loans and has commendable performance for high-risk loans.

    Model with Resampled Data: Displays almost perfect accuracy, a common outcome when oversampling is used to balance the training data, enhancing the model's ability to identify the minority class.

    Recommendation: Considering the significance of accurately detecting high-risk loans, a model with superior recall for the high-risk category is recommended.
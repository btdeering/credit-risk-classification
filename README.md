# credit-risk-classification
Module 12 Report
Overview of the Analysis

In the challenge, we embarked on a mission to leverage machine learning to better understand and predict loan risks. This was crucial as the correct classification of loans as either "healthy" or "high-risk" can greatly influence an institution's financial health.

Purpose of the Analysis:
The primary goal was to determine which loans might be at risk. As loan default could lead to significant financial losses, predicting this is of paramount importance.

Data Overview:
The dataset encompassed various financial metrics, such as loan size, interest rate, borrower income, debt-to-income ratio, among others. Our main task was to predict the loan_status variable, which categorized loans as either healthy (0) or high-risk (1).

Machine Learning Process:

    Data Preprocessing: We cleaned and preprocessed the data, ensuring it was suitable for machine learning.
    Data Splitting: We divided our data into training and testing sets.
    Model Training: We trained a Logistic Regression model on the original data and another on oversampled data to address the imbalance in the dataset.
    Evaluation: Models were evaluated based on accuracy, precision, and recall metrics.

Methods Used:

    Model: Logistic Regression
    Resampling: Random OverSampling for the second model

Results

    Original Logistic Regression Model:
        Accuracy Score: Approximately 99%
        Precision:
            Healthy loans (label 0): 1.00
            High-risk loans (label 1): 0.85
        Recall:
            Healthy loans (label 0): 0.99
            High-risk loans (label 1): 0.91

    Logistic Regression Model with Oversampled Data:
        Accuracy Score: Approximately 99.4%
        Precision:
            Healthy loans (label 0): 1.00
            High-risk loans (label 1): 0.84
        Recall:
            Healthy loans (label 0): 0.99
            High-risk loans (label 1): 0.99

Summary

Upon evaluation:

    Both models present impressive accuracy scores. However, due to the imbalanced nature of the dataset, looking solely at accuracy might be misleading.

    The Logistic Regression Model trained with oversampled data seems to perform the best, particularly in terms of recall for high-risk loans. In the lending domain, the cost of missing a high-risk loan (false negative) could be substantial, making recall an essential metric.

Considering the results and the context, we recommend the Logistic Regression Model with Oversampled Data for deployment. Its heightened ability to detect high-risk loans makes it a prudent choice for the company, ensuring minimal exposure to potential loan defaults.

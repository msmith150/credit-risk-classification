# Credit Risk Analysis Report

## Overview

The purpose of this analysis is to evaluate the performance of a machine learning model used to predict loan status based on various features in the `lending_data.csv` dataset. The goal is to predict the creditworthiness of borrowers in order to determine whether or not a loan should be approved, using a variety of features such as loan amount, term, and applicant characteristics. The analysis involves building a Logistic Regression model, training it on historical data, and evaluating its performance using standard classification metrics.

## Results

The performance of the Logistic Regression model was evaluated using the following metrics:

- **Accuracy Score**: The proportion of correct predictions made by the model out of all predictions.
- **Precision**: The ratio of correctly predicted positive observations to the total predicted positives.
- **Recall**: The ratio of correctly predicted positive observations to all actual positives.

### Performance Metrics:

- **Accuracy**: 0.807  
  This means the model correctly predicted loan status 80.7% of the time on the testing dataset.

- **Precision**: 0.725  
  This indicates that when the model predicts a loan as "approved" (positive class), it is correct 72.5% of the time.

- **Recall**: 0.651  
  This means the model correctly identified 65.1% of all loans that were actually approved.

### Confusion Matrix:
The confusion matrix displays the true positives (correctly predicted approved loans), false positives (incorrectly predicted approved loans), true negatives (correctly predicted denied loans), and false negatives (incorrectly predicted denied loans). This is a useful tool to understand where the model is making mistakes.

## Summary

Based on the results from the Logistic Regression model, key takeaways are as follows:

- The model has a reasonably high accuracy of 80.7%, meaning it correctly predicts loan approval status most of the time.
- Precision (0.725) and recall (0.651) suggest that the model's ability to correctly predict both "approved" loans (precision) and "approved" loans in general (recall) could be improved.
- In practice, these performance metrics suggest that while the model performs well overall, there is room for improvement, particularly in reducing false positives (i.e., predicting a loan as approved when it was actually denied) and false negatives (i.e., predicting a loan as denied when it was approved).

### Recommendation:
Given the moderate performance, the model could be used as a baseline for decision-making, but further refinement or testing with other algorithms (e.g., Random Forest, XGBoost, or Neural Networks) may yield better results. The model's relatively low recall rate might be a concern if the company is more focused on identifying all approved loans (to maximize loan issuance) rather than minimizing errors in predicting denied loans. 

It is recommended to test additional models and perform hyperparameter tuning to enhance the overall prediction capability, especially with regard to recall and precision.

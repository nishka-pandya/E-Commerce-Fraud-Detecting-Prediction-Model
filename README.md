# E-Commerce-Fraud-Detecting-Prediction-Model


# Research Question / Problem Statement 

**What methods can be used to detect fraud in E-Commerce platforms?**

**List of Datasets:**
1)  - This is a dataset from Kaggle that contains information that can help determine whether there is fraud. I chose it because it is a dataset from an e-commerce platform that has data on thousands of users. It has a lot of columns that would help determine fraudulent behavior so I can explore and experiment with many columns.
  
# Summary of Dataset Use 

**Model 1: Decision Tree**

1) Used Kaggle E-Commerce Fraud Detection Dataset
2) Metric(s) used to evaluate the model: accuracy, recall, precision, F1 score.
3) Key Insight(s): The highest feature importance was "account_age_days", which did not have a high correlation to "is_fraud", while the lowest feature importance was "cvv_result", which was surprising because it had the highest correlation with "is_fraud".
4) Used AI/LLMs to ask conceptual questions such as how to determine whether a model is effective based on accuracy and F1 score with general examples so I can better understand metrics.

**Model 2: Random Forests**

1) Used Kaggle E-Commerce Fraud Detection Dataset
2) Metric(s) used to evaluate the model: accuracy, F1 score, precision, recall, and confusion matrix.
3) Key Insight(s): In the confusion matrix, the model detected a lot of true negatives and true positives compared to false positives and false negatives.
4) Used AI/LLMs to ask conceptual questions such as how to determine whether a model is effective based on accuracy and F1 score with general examples so I can better understand metrics.


# Overall AI/LLM Usage 

1) Used it to understand conceptual questions such as how to determine whether a model is effective based on accuracy and F1 score with general examples so I can better understand metrics.
2) Used it to understand what types of verification can be used instead of only avs_match and cvs_result, such as digital fingerprints.
3) Used it to understand how I could potentially improve F1 score and recall.
4) For the improvement in the model section of the presentation (next steps), ChatGPT recommended using gradient modeling.

# Results 

Overall, both machine learning models had high accuracy for both testing and training that were not overfitting or underfitting. However, it is important to note that the F1 score and recall for both the training and testing sets for both models had a high percentage around 30%. The random forest model's confusion matrix detected most true positives and true negatives compared to any false. In the future, it is recommended to try more advanced models to increase F1 score and recall. According to the exploratory data analysis, shipping distance and amount have a high positive correlation and can be further explored in individual user accounts to detect more patterns.

# Conclusion and Recommendations 

1. Random Forests: A model to use for simplicity while providing accuracy, as seen in metrics and correlation.
2. Large distance between billing and shipping address: If the shipping distance is large, implement further verifications that notify the user through email, phone, messages, etc.
3. Identity Verification: Besides "CVV_result" and "AVS_match", other verifications can strengthen the chances of identifying fraud quickly, such as digital fingerprints.
4. Compare amount of transaction to average amount: If the transaction amount is larger, implement further verifications that notify the user immediately through email, phone, messages, etc. It is important to further analyze larger transactions than the user's average transactions because the amount is positively correlated to is_fraud.

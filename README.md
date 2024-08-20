# Module 12 Report Template

## Overview of the Analysis

Using historical lending activity from a peer-to-peer lending services company, I’ve trained and evaluated a model to identify creditworthiness of borrowers. This simple ai split the dataset to fit a regression model. You can view the code here: C’mon Over Y’all

## Results

Class 0 (Healthy Loan):

* Precision: 1.00 (perfect precision, no false positives)
* Recall: 0.99 (very high recall, only 1% of actual healthy loans are misclassified)
* F1-score: 1.00 (perfect F1-score, indicating excellent balance between precision and recall)
The model is extremely accurate in predicting healthy loans (class 0). It correctly identifies almost all healthy loans (99% recall) and doesn't misclassify any healthy loans as high-risk loans (100% precision).

Class 1 (High-Risk Loan):

* Precision: 0.85 (good precision, but some false positives)
* Recall: 0.91 (good recall, but some high-risk loans are missed)
* F1-score: 0.88 (good F1-score, but not as high as class 0)
The model is good, but not excellent, in predicting high-risk loans (class 1). It correctly identifies most high-risk loans (91% recall), but also misclassifies some healthy loans as high-risk loans (15% false positives, as indicated by the precision).

## Summary

The model is generally very good, with high accuracy and excellent performance on the majority class (healthy loans). However, there's room for improvement in predicting high-risk loans. The model tends to be more cautious and predicts more false positives (healthy loans as high-risk loans) than false negatives (missing high-risk loans).

To improve the model, I'm considering:

* Collecting more data on high-risk loans to improve the model's performance on this class.
* Adjusting the model's hyperparameters or using techniques like class weighting to reduce the bias towards the majority class.
* Exploring other models or ensemble methods that can better handle class imbalance.
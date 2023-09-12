
**UCB Data Analysis Module 20**
# Credit-Risk-Classification Challenge

---------------
## Analysis of Machine Learning Models for Loan Prediction

#### I.  OVERVIEW

This analysis aims to evaluate the performance of machine learning models for predicting the outcome of healthy and high-risk loans. Two machine learning models were employed for this task: a logistic regression model with the original dataset (Model 1) and a logistic regression model trained on resampled data (Model 2).  The latter makes use of the 'RandomOverSampler' from the 'imbalanced-learn' library to address class imbalance in the dataset.

The following measures serve as the basis for comparison between the two models:
1.  **Balanced Accuracy**:  A single value representing the model's predictive performance while taking into account class imbalance.
2.  **Precision Score**:  A measure of the proportion of true positive predictions among all positive predictions for each class. 
3.  **Recall Score**:  Measures the proportion of true positive predictions among all instances for each class. 
4.  **F1-Score**:  Equivalent to the calculated mean of the precision and recall scores.

#### II. RESULTS

**Machine Learning Model 1 (original data):**
- Overall Accuracy: 99%
- Balanced Accuracy Score: 94.4%
- Precision Score (Class 0): 100%
- Precision Score (Class 1): 87%
- Recall Score (Class 0): 100%
- Recall Score (Class 1): 89%
- F1-Score (Class 0): 100%
- F1-Score (Class 1): 88%

**Machine Learning Model 2 (resampled data):**

- Overall Accuracy: 100%
- Balanced Accuracy Score: 94.4%
- Precision Score (Class 0): 100%
- Precision Score (Class 1): 87%
- Recall Score (Class 0): 100%
- Recall Score (Class 1): 100%
- F1-Score (Class 0): 100%
- F1-Score (Class 1): 93%

#### III. SUMMARY

Model 1 achieved a high overall accuracy of 99%, suggesting strong performance in making predictions for both healthy and high-risk loans. However, it exhibited slightly reduced prediction and recall scores for Class 1 (high-risk loans), suggesting there may be room for improvement in identifying these high-risk cases.

Model 2, which incorporated resampled training data to address class imbalance, displayed remarkable performance as a predictive model with overall accuracy of 100%.  It achieved perfect precision, recall and F1 scores for Class 0 (healthy loans) and a notably improved recall score for Class 1. Furthermore, the F1-score for Class 1 also increased to 93%, which indicates the model attained superior balance between precision and recall.

Based on these results, Model 2 (with resampled training data) is recommended as the best fit model for this dataset.  Not only does it deliver increased performance for identifying high-risk loans, it also demonstrates superior effectiveness by addressing class imbalance through data resampling.  

--------------
#### Contents of Repository:
- Code Script (see Credit_Risk folder)
  - 1 x IPython Notebook file (credit_risk_classificiation.ipynb)
- Resources Folder
  - 1 x .csv file (lending_data.csv) - provided
- 1 x README file

-------------------
#### Contributions:  
N/A

------------------
#### License:
[MIT](https://choosealicense.com/licenses/mit/)

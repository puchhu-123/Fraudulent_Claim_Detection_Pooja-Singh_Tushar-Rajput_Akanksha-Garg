FRAUDULENT_CLAIM_DETECTION_CASE-STUDY

Problem Statement:-


Global Insure, a leading insurance company, processes thousands of claims annually. However, a significant percentage of these claims turn out to be fraudulent, resulting in considerable financial losses. The company’s current process for identifying fraudulent claims involves manual inspections, which is time-consuming and inefficient. Fraudulent claims are often detected too late in the process, after the company has already paid out significant amounts. Global Insure wants to improve its fraud detection process using data-driven insights to classify claims as fraudulent or legitimate early in the approval process. This would minimise financial losses and optimise the overall claims handling process.


Business Objective:-

Global Insure wants to build a model to classify insurance claims as either fraudulent or legitimate based on historical claim details and customer profiles. By using features like claim amounts, customer profiles and claim types, the company aims to predict which claims are likely to be fraudulent before they are approved.


Based on this assignment, you have to answer the following questions:

● How can we analyse historical claim data to detect patterns that indicate fraudulent claims?
● Which features are most predictive of fraudulent behaviour? 
● Can we predict the likelihood of fraud for an incoming claim, based on past data? 
● What insights can be drawn from the model that can help in improving the fraud detection process?


Assignment Tasks:-

We need to perform the following steps for successfully completing this assignment:

-Data Preparation

-Data Cleaning

-Train Validation Split 70-30

-EDA on Training Data

-EDA on Validation Data (optional)

-Feature Engineering

-Model Building

-Predicting and Model Evaluation


Data Overview:-

-Rows: 1000 -Columns: 40



Evaluation and Conclusion:-

Random Forest Model vs Logistic Regression

After evaluating the performance of the tuned Random Forest model on the validation dataset, we observed the following:

-Accuracy: 76.92% -Precision: 57.14% -Recall (Sensitivity): 11.76% -Specificity: 97.25% -F1 Score: 0.1951 While the Random Forest model shows high specificity and slightly better accuracy than the Logistic Regression model, its recall is extremely poor. With a recall of just 11.76%, it fails to identify the majority of actual fraud cases — a critical shortcoming in fraud detection where missing fraudulent claims can be costly.

In contrast, the Logistic Regression model, though slightly lower in accuracy (73.43%), achieves a much higher recall of 82.35% and a more balanced F1 score of 0.5957. This indicates that it is significantly better at detecting fraudulent claims, even if it occasionally misclassifies some non-fraud cases.



Conclusion:-

Given the problem context, where detecting fraud is more important than avoiding false positives, the Logistic Regression model outperforms the tuned Random Forest model. Therefore, Logistic Regression should be preferred for final deployment in this case.

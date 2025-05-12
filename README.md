# BANK-CUSTOMER-CHURN-PREDICTION

![bank ppple](https://github.com/user-attachments/assets/77de0350-845e-44d7-a909-51ae85fb4510)

Photo by <a href="https://unsplash.com/@cardmapr?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">CardMapr.nl</a> on <a href="https://unsplash.com/photos/person-holding-black-remote-control-PP4LPGM3gHg?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
      

Business Problem Statement

In the competitive landscape of the banking industry, customer churn poses a critical business challenge with significant financial and social repercussions. Banks face substantial revenue loss and increased acquisition costs when customers terminate their accounts—a phenomenon directly impacting the institution's growth and profitability.

By applying analytics to predict and analyze churn patterns through customer data like demographics, transaction behaviors, and service interactions, banks can identify at-risk individuals and implement targeted retention strategies. Such data-driven solutions not only have the potential to enhance customer satisfaction and loyalty, reducing churn, but they also promote a positive brand reputation and community trust.

The financial benefits of these analytical applications include stabilizing the bank's revenue stream and minimizing the costs associated with customer turnover. By identifying at-risk customers beforehand, banks can take proactive measures to retain them, thereby improving customer satisfaction and profitability. Socially, a lower churn rate can reflect a bank's commitment to its customers, fostering a supportive financial environment and driving organic growth through word-of-mouth endorsements. Therefore, leveraging analytics to reduce customer churn can catalyze both the economic stability and social standing of a financial institution.


Summarizing the better model based on each metric :

Precision: Precision measures the proportion of positive identifications that were actually correct. The Random Forest model has the highest precision for Class 1 (exited), indicating that when it predicts a customer will churn, it is more likely to be correct compared to other models.

Recall: Recall, or sensitivity, measures the proportion of actual positives that were correctly identified. The Random Forest and Boosted Tree models have a higher recall for Class 0 (not exited), but they have a lower recall for Class 1 (exited) compared to other models. This means they are good at identifying customers who did not churn but not as good at identifying those who did churn.

F1-Score: The F1-score is the harmonic mean of precision and recall, which balances the two metrics. Among the models, the Random Forest and Boosted Tree models have higher F1-scores for Class 0 but a lower score for Class 1 compared to other models, indicating they are better overall when considering both precision and recall but still not ideal for identifying churned customers (Class 1).

ROC AUC: Based on the ROC curve and AUC values:Random Forest and Boosted Tree models have the highest AUC (0.85), indicating they are the best among the ones presented for distinguishing between the customer classes overall. The Decision Tree model follows them with an AUC of 0.80. Logistic Regression has an AUC of 0.69. Naive Bayes and KNN are the weakest, with AUCs of 0.54 and 0.58, respectively. Best Model Based on Metrics Recall: No clear winner; it depends on the class of interest. For Class 0, Random Forest and Boosted Tree are best. For Class 1, despite the lower AUC, Decision Tree, Logistic Regression, KNN, and Naive Bayes have higher recalls. Precision: Random Forest outperforms the other models for Class 1. F1-Score: Random Forest and Boosted Tree have the best F1-scores for Class 0, but all models have relatively poor scores for Class 1. ROC AUC: Random Forest and Boosted Tree are the best, but Random Forest has a slightly better precision, giving it a slight edge overall.

Conclusion: 

Considering all the metrics, the Random Forest model is the best performing model for this bank customer churn prediction task based on the provided data. It has a good balance between precision and recall, especially for predicting customers who do not churn (Class 0), and it has the highest AUC, suggesting strong overall performance. However, there is still room for improvement in identifying churned customers (Class 1), as indicated by lower recall and F1-scores. Banks should consider using the Random Forest model for initial churn prediction efforts but might want to combine it with other strategies or further model tuning to better identify at-risk customers.

# churn-prediction
# Customer Churn Prediction & Retention Strategy
We started by importing the data, then verified the data types for the columns, performed data cleaning, handled null values, and considered outliers as a starting point for the analysis process.
This was followed by a simple descriptive analysis to study the features and their effects, as well as to gain a better understanding and familiarity with the data, as shown in the code.
We then created two prediction models, each in two forms: a normal image and an image, using RandomizedSearchCV. Based on the results of several metrics, we selected the logistic regression model with RandomizedSearchCV as the most appropriate model among the tested models.
Based on the above, we reached the following recommendations:

#Recommendations

1- Focus on customer tenure, total charges, and monthly charges:

The significant impact of each of these factors on customer churn, especially for new customers, warrants special attention for new customers or customers with high monthly charges but low total charges, as they are the most vulnerable to churn.



2- Importance of contract type:

It can be noted that customers with short-term contracts are more vulnerable to churn. The attractiveness of long-term contracts can be increased as the company deems appropriate.



3- Fiber optic cable service:

Although the service is advanced and supposed to be an attractive factor, it poses a serious risk of churn. The quality of the service, its prices, the competitive market, as well as the maintenance and associated services should be reviewed.



It may be best to study the entire service to identify the causes of the discrepancy.



4- Electronic Checks as a Payment Method:

The results demonstrate that this service is associated with an increased dropout rate. This requires further study to determine the reason for this association, whether there is a problem with the service, the suitability of alternative services, and whether alternatives exist and should be encouraged.



5- Online Security and Technical Support Services:

Customers who subscribe to security and technical support services are less likely to drop out. These services should be encouraged more, and awareness of their importance should be raised.



6- Balancing Recall and Precision in Intervention:



Our model achieved a very high Recall (0.78) compared to Precision (0.51).



Recommendation: This means that the company will detect 78% of customers who will actually drop out, which is excellent. However, approximately 49% of customers predicted to drop out by the model will not actually drop out (false alarms). An intervention strategy (such as phone calls or special offers) should be designed to be cost-effective, as it will be applied to a significant number of customers who will not churn. A company can focus on low-cost interventions for false alarms (such as emails or text messages) and allocate more expensive interventions (such as personal calls or significant discounts) to customers with a very high churn probability based on the model's predicted likelihood score.

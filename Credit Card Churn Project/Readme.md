# Credit Card Users Churn Prediction

## Problem Statement

![Credit Card Image](Credit-Cards.jpg)

---

### Business Context

The Thera bank recently saw a steep decline in the number of users of their credit card, credit cards are a good source of income for banks because of different kinds of fees charged by the banks like annual fees, balance transfer fees, and cash advance fees, late payment fees, foreign transaction fees, and others. Some fees are charged to every user irrespective of usage, while others are charged under specified circumstances.

Customers’ leaving credit cards services would lead bank to loss, so the bank wants to analyze the data of customers and identify the customers who will leave their credit card services and reason for same – so that bank could improve upon those areas

As a Data scientist at Thera bank, I need to come up with a classification model that will help the bank improve its services so that customers do not renounce their credit cards

### Data Description

* CLIENTNUM: Client number. Unique identifier for the customer holding the account
* Attrition_Flag: Internal event (customer activity) variable - if the account is closed then "Attrited Customer" else "Existing Customer"
* Customer_Age: Age in Years
* Gender: Gender of the account holder
* Dependent_count: Number of dependents
* Education_Level: Educational Qualification of the account holder - Graduate, High School, Unknown, Uneducated, College(refers to college student), Post-Graduate, Doctorate
* Marital_Status: Marital Status of the account holder
* Income_Category: Annual Income Category of the account holder
* Card_Category: Type of Card
* Months_on_book: Period of relationship with the bank (in months)
* Total_Relationship_Count: Total no. of products held by the customer
* Months_Inactive_12_mon: No. of months inactive in the last 12 months
* Contacts_Count_12_mon: No. of Contacts in the last 12 months
* Credit_Limit: Credit Limit on the Credit Card
* Total_Revolving_Bal: Total Revolving Balance on the Credit Card
* Avg_Open_To_Buy: Open to Buy Credit Line (Average of last 12 months)
* Total_Amt_Chng_Q4_Q1: Change in Transaction Amount (Q4 over Q1)
* Total_Trans_Amt: Total Transaction Amount (Last 12 months)
* Total_Trans_Ct: Total Transaction Count (Last 12 months)
* Total_Ct_Chng_Q4_Q1: Change in Transaction Count (Q4 over Q1)
* Avg_Utilization_Ratio: Average Card Utilization Ratio

#### What Is a Revolving Balance?

- If we don't pay the balance of the revolving credit account in full every month, the unpaid portion carries over to the next month. That's called a revolving balance


##### What is the Average Open to buy?

- 'Open to Buy' means the amount left on your credit card to use. Now, this column represents the average of this value for the last 12 months.

##### What is the Average utilization Ratio?

- The Avg Utilization Ratio represents how much of the available credit the customer spent. This is useful for calculating credit scores.


##### Relation b/w Avg_Open_To_Buy, Credit_Limit and Avg_Utilization_Ratio:

- ( Avg_Open_To_Buy / Credit_Limit ) + Avg_Utilization_Ratio = 1

---

# Business Insights and Conclusions

**Model Insights:**

The final model achieved good and consistent peformance on training, validating and testing data in each of the validating metrics:

- Accuracy Training vs Validation scores: 0.976, 0.955

- Recall Training vs Validation scores: 0.980, 0.899

- Precision Training vs Validation sores: 0.972, 0.835

- F1 Training vs Validation scores: 0.976, 0.866

- Cross Validation score: 0.9488217976101136.

The consistency indicates that it will continue to perform well in production.



**Business Insights**

Complete analysis of the data revealed that:

- customers holding a Blue card account for 93% of all attrited card holders. As the intent is to keep current card holders I would conclude that further analysis ought to be done to determine what about the card leads to attrition.

- Customers with income less that $40k account for 38% of attrition rates.

- This correlates with that fact that women make up 57% of attrition rates with respect to gender and they also account for a greater portion of those in the less that $40k income category.

- Those with credit limits $5k or less are also more likely to renounce their cards, likely due to the small amount being easy to payoff or transfer to another institution.

- Another flag to indicate attrition is the number of contacts a customer has with the bank. The higher the number of contacts, the more likely to leave, with 6 contacts in the preceeding 12 months being the magic number, as all attrited customers with 6 contact with the bank left. This may indicate a dissatisfaction with something pertaining to the card that isn't being resolved.
![bank image](bank-image.jpg)

### Context

AllLife Bank is a US bank that has a growing customer base. The majority of these customers are liability customers (depositors) with varying sizes of deposits. The number of customers who are also borrowers (asset customers) is quite small, and the bank is interested in expanding this base rapidly to bring in more loan business and in the process, earn more through the interest on loans. In particular, the management wants to explore ways of converting its liability customers to personal loan customers (while retaining them as depositors).

A campaign that the bank ran last year for liability customers showed a healthy conversion rate of over 9% success. This has encouraged the retail marketing department to devise campaigns with better target marketing to increase the success ratio.

As a Data scientist at AllLife bank, I have to build a model that will help the marketing department to identify the potential customers who have a higher probability of purchasing the loan.

---

### Objective

To predict whether a liability customer will buy personal loans, to understand which customer attributes are most significant in driving purchases, and identify which segment of customers to target more.

---

### Data Dictionary
* `ID`: Customer ID
* `Age`: Customer’s age in completed years
* `Experience`: #years of professional experience
* `Income`: Annual income of the customer (in thousand dollars)
* `ZIP Code`: Home Address ZIP code.
* `Family`: the Family size of the customer
* `CCAvg`: Average spending on credit cards per month (in thousand dollars)
* `Education`: Education Level. 1: Undergrad; 2: Graduate;3: Advanced/Professional
* `Mortgage`: Value of house mortgage if any. (in thousand dollars)
* `Personal_Loan`: Did this customer accept the personal loan offered in the last campaign? (0: No, 1: Yes)
* `Securities_Account`: Does the customer have securities account with the bank? (0: No, 1: Yes)
* `CD_Account`: Does the customer have a certificate of deposit (CD) account with the bank? (0: No, 1: Yes)
* `Online`: Do customers use internet banking facilities? (0: No, 1: Yes)
* `CreditCard`: Does the customer use a credit card issued by any other Bank (excluding All life Bank)? (0: No, 1: Yes)

---

# Insights from the data:
* The highest personal loan interest from those with a mortgage value is customers with mortgage loan values between 0-200k.
* The highest loan interest taking into consideration income levels is those with incomes between $130K-180K.
* The highest personal loan interest taking into consideration level of education is those in education categories 2 and 3.
* Families of more than 2 members are more likely to accept a personal loan
* Those with a Securities account or CD are more likely to accept a personal loan.
* The most ideal age range for interest in a personal loan is between 35-55 yrs.
* The 4 greatest contributors to the likelihood of accepting a personal loan are Income, Family size, and Education levels 2 & 3

# Business Recommendations
* The ZIPCode column could potentially be a very valuable information source. However, there isn't nearly enough data in this set for it to make any difference in any of the predictive models. I would recommend a bigger data set if one is available.
* The model with the highest test Recall value is the pre-pruned model. We're most concerned about True positive predictions and thus want to limit False negatives. This model does the best on Recall with a 79% success rate. It also scores really well on Accuracy: 98%, Precision: 100% and F1: 88%.
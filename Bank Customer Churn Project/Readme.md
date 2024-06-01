<center><font size=6>Bank Customer Churn Prediction</font></center>

!['Bank desk image'](bank-image.jpg)

## Problem Statement

### Context

Businesses like banks which provide service have to worry about problem of 'Customer Churn' i.e. customers leaving and joining another service provider. It is important to understand which aspects of the service influence a customer's decision in this regard. Management can concentrate efforts on improvement of service, keeping in mind these priorities.

### Objective

You as a Data scientist with the  bank need to  build a neural network based classifier that can determine whether a customer will leave the bank  or not in the next 6 months.

---

### Data Dictionary

* CustomerId: Unique ID which is assigned to each customer

* Surname: Last name of the customer

* CreditScore: It defines the credit history of the customer.
  
* Geography: A customer’s location
   
* Gender: It defines the Gender of the customer
   
* Age: Age of the customer
    
* Tenure: Number of years for which the customer has been with the bank

* NumOfProducts: refers to the number of products that a customer has purchased through the bank.

* Balance: Account balance

* HasCrCard: It is a categorical variable which decides whether the customer has credit card or not.

* EstimatedSalary: Estimated salary

* isActiveMember: Is is a categorical variable which decides whether the customer is active member of the bank or not ( Active member in the sense, using bank products regularly, making transactions etc )

* Exited : whether or not the customer left the bank within six month. It can take two values
** 0=No ( Customer did not leave the bank )
** 1=Yes ( Customer left the bank )

---

## Actionable Insights and Business Recommendations

- About 20% of all customers churn. The Bank concerned with identifying customers who may leave for another in the next 6 months can deploy this model. This model is simple and resource friendly with tested weighted recall of 86%.
- Consider better marketing strategies with a focus on customers in Germany. Germany has the highest churn rate of 32%, which is double that of other countries.
- Consider more inclusive marketing and outreach strategies as women church at a higher rate than men over all and make up the biggest group switching banks in every country included in this data.
- Credit card holding customers are less likely to churn than their counterparts, so targeted card campaigns could reduce churn rates.
- Track and reach out to inactive customers. Almost 30% of all inactive customers churn. Consider outreach campaigns.
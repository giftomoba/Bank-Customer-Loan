## Description
### Context

AllLife Bank is a US bank that has a growing customer base. The majority of these customers are liability customers (depositors) with varying sizes of deposits. The number of customers who are also borrowers (asset customers) is quite small, and the bank is interested in expanding this base rapidly to bring in more loan business and in the process, earn more through the interest on loans. In particular, the management wants to explore ways of converting its liability customers to personal loan customers (while retaining them as depositors).

A campaign that the bank ran last year for liability customers showed a healthy conversion rate of over 9% success. This has encouraged the retail marketing department to devise campaigns with better target marketing to increase the success ratio.

You as a Data scientist at AllLife bank have to build a model that will help the marketing department to identify the potential customers who have a higher probability of purchasing the loan.
## Objective

- To predict whether a liability customer will buy a personal loan or not.
- Which variables are most significant.
- Which segment of customers should be targeted more.



## Data Description

The data provided contains records of customers finantial records and also their loan status, that is whether they accepted loan or not.

## Data Dictionary
* ID: Customer ID
* Age: Customer’s age in completed years
* Experience: #years of professional experience
* Income: Annual income of the customer (in thousand dollars)
* ZIP Code: Home Address ZIP code.
* Family: the Family size of the customer
* CCAvg: Average spending on credit cards per month (in thousand dollars)
* Education: Education Level. 1: Undergrad; 2: Graduate;3: Advanced/Professional
* Mortgage: Value of house mortgage if any. (in thousand dollars)
* Personal_Loan: Did this customer accept the personal loan offered in the last campaign?
* Securities_Account: Does the customer have securities account with the bank?
* CD_Account: Does the customer have a certificate of deposit (CD) account with the bank?
* Online: Do customers use internet banking facilities?
* CreditCard: Does the customer use a credit card issued by any other Bank (excluding All life Bank)?

## Link to access the jupyter notebook file for this project:
https://github.com/giftomoba/Bank-Customer-Loan/blob/main/Personal%20Loan%20Project%20-%20Submit.ipynb

## Key Project Analysis and Visualization:

![loan 1](https://github.com/giftomoba/Bank-Customer-Loan/assets/124467481/40f0e887-101d-4378-8d45-a2083dd84365)
 ![loan cat](https://github.com/giftomoba/Bank-Customer-Loan/assets/124467481/6ef6790a-c086-4e8f-b169-dd7c0ba54cbf)
- 90.4% did not take loan while only 9.6% took loan.
- Some customers with much higher income (above $150,000) didn't take loan even though they earned more income than those who did.

![loan income](https://github.com/giftomoba/Bank-Customer-Loan/assets/124467481/3cd0a5fa-1270-4af5-8943-4331687eab34)
- Most of the customers who took loan earn above $100,000 while most of those who didn't earn lesser.

## Model Results:
![loan train](https://github.com/giftomoba/Bank-Customer-Loan/assets/124467481/d2f1ab31-1473-45ea-80c4-3ecd74b76181)
![loan Test](https://github.com/giftomoba/Bank-Customer-Loan/assets/124467481/3ee75009-669b-446e-8987-2645ddb727bb)

![loan conf](https://github.com/giftomoba/Bank-Customer-Loan/assets/124467481/0710c195-2ea3-462e-942e-239a97594485)

![loan ,odel](https://github.com/giftomoba/Bank-Customer-Loan/assets/124467481/cbaa8c4e-441e-49a6-8112-7160906ff904)
- Model still performed well for both training and testing, with high recall values of 100%.
- Model can effectively be deployed to predict whether a customer will accept the loan.
- Model can be deployed because it fully satifies the objective of the bank and is less costly to apply due to it's smaller dimension.

## Recommendations:
- From the analysis shown above, it is clear that most of the customers who accepted the loan are high earners above 100,000 dollars.
- Hence, the bank should focus more on high income earners above $100,000, especially the few who earn higher than this amount but didn't accept the loan.

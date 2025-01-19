# Customer Churn Analysis for a Fictional Internet and Phone Service Provider

## I. Introduction

Customer churn is a pressing issue for businesses in the competitive telecommunications industry. Churn, the
process where customers discontinue their service, often results from dissatisfaction or more attractive offerings
by competitors. This report analyses a dataset of over 7,000 customer records from a fictional internet and phone
service provider in California. The goal is to identify patterns and key factors contributing to customer churn,
with a focus on demographic trends, service preferences, payment behaviour, and satisfaction scores. These
insights will form the basis for actionable strategies to improve customer retention.

## II. Data

The dataset consists of over 7,000 records detailing customer demographics, service usage, payment behaviour,
and satisfaction levels. Each record provides information such as age, marital status, number of dependants, and
location, alongside service-related data like internet type, contract type, and online security options. Payment
behaviour, including methods, monthly charges, tenure, and billing preferences, is also documented.
Behavioural metrics like satisfaction scores, referrals, and churn likelihood offer deeper insights into customer
decision-making. Finally, the dataset captures churn status, reasons for churn, and churn probabilities. This rich
dataset enables a comprehensive analysis of factors influencing customer churn and serves as a foundation for
predictive modelling and strategic planning.

## III. Analysis

### A. Churn rate

An analysis of churn data reveals that competitive offerings are the primary reason for churn, accounting for
45% of all cases. Satisfaction scores play a crucial role in determining churn likelihood, with all customers
scoring 4 or above continuing their service. Conversely, nearly all customers with scores of 1 or 2 have churned,
while 16.1% of those with a score of 3 have also left the company. This correlation highlights the importance of
customer satisfaction in retention strategies.

![](https://github.com/RaphaelSanbar/Churn_Rate/blob/f58992c3d805798a5ef7f7232b61cb30b36b1c29/Screenshot%202025-01-03%20194355.png)

Fig. 1. Bar chart illustrating the distribution of customer churn reasons, with a significant majority attributed to competition, highlighting its dominance as the primary driver of customer churning.

#### 3.1 Customer Information

The churn rate remains consistent at around 25% across most age groups but increases to 40% for customers
aged 65 and older. While no correlation is observed between gender and churn, marital status emerges as a
significant factor, with married customers being 12% less likely to churn than single customers. Dependants also
influence churn rates, with those having no dependants experiencing a 35.55% churn rate. This figure rises
steeply as the number of dependants increases, culminating in a 50% churn rate for customers with seven
dependants.

Fig. 2. Area chart showing the relative churn rate by age, emphasizing a sharp decline in customer retention among customers aged 65 and older.

#### 3.2 Online Services

The adoption of premium tech support and online security services is associated with slight reductions in churn
rates. However, customers with fibre-optic internet services exhibit a significantly higher churn rate of 40.72%.
This suggests that issues related to fibre-optic service may be contributing to customer dissatisfaction.

#### 3.3 Payment Information

Payment method and contract type are strong predictors of churn. Customers who pay via electronic check have
a churn rate of 45.29%, far exceeding the 16.71% average for other payment methods. Similarly, those on
month-to-month contracts face a churn rate of 45.84%, in stark contrast to the 10.71% rate for one-year
contracts and the 2.55% rate for two-year contracts. These findings underline the role of financial and
contractual stability in customer retention.

#### 3.4 Account Information

An inverse linear relationship is evident between both tenure and number of referrals with churn rates. Longer-
tenured customers and those who have referred others to the company are significantly less likely to churn. 
Among promotional offers, Offer E stands out with a high churn rate of 52.92%. In contrast, Offer A, though
less popular, has an impressively low churn rate of 6.73%. This discrepancy indicates potential issues with the
design or implementation of Offer E.

Fig. 3. Bar chart depicting the churn rate relative to the number of referrals, revealing a clear trend of decreasing churn rates as the number of referrals increases.

## B. Satisfaction score

Satisfaction scores are a direct indicator of customer retention. Higher scores correlate with lower churn rates,
with the notable exception of customers opting for online security services. Despite having lower average
satisfaction scores, these customers exhibit reduced churn rates, suggesting that specific features might offset
dissatisfaction in other areas.

Fig. 4. Pie chart illustrating the distribution of satisfaction scores among customers with and without online security, highlighting noticeably lower satisfaction scores for those with online security.

## IV. Conclusion

The findings from this analysis highlight several key areas for intervention to reduce churn and improve
customer retention. Demographically, older customers and those with multiple dependants are at a higher risk of
churning. To address this, the company could introduce targeted retention campaigns, such as family plans or
senior discounts, to appeal to these vulnerable segments.
Service-related factors, particularly fibre-optic internet, require immediate attention. An inquiry into fibre-optic
service quality, followed by improvements in reliability and customer support, could significantly reduce churn
in this group. Furthermore, the promotion of premium tech support and online security services, which are
associated with lower churn rates, should be emphasized in marketing efforts.

Financial stability is another critical factor. Customers on month-to-month contracts or using electronic checks
for payment have the highest churn rates. Transitioning these customers to longer-term contracts or promoting
more stable payment methods, such as credit cards or direct debits, could enhance retention. Offering incentives
for switching payment methods or signing longer contracts would be an effective strategy.
Referral programs and promotional offers also play a vital role. The success of Offer A, combined with the high
churn associated with Offer E, suggests that the latter needs re-evaluation. Revising Offer E to better align with
customer needs, while continuing to promote Offer A’s benefits, could improve customer retention rates.
Additionally, enhancing the referral program and rewarding loyal customers for bringing in new business could
further reduce churn.
Finally, satisfaction scores offer a clear benchmark for customer experience. Targeting customers with middling
scores (e.g., 3) with personalized support or special offers could pre-empt churn. Improving service quality,
addressing complaints swiftly, and maintaining open communication with customers are essential for fostering
satisfaction and loyalty.
By implementing these strategies, the company can proactively address churn, improve customer satisfaction,
and ensure long-term success in a competitive market.

### V. Appendix

#### Appendix A: Data Cleaning Steps:

Created relationships between 5 tables.

Changed column data types to better suit the data.

#### Appendix B: Tools used included:

MySQL: For data extraction, involving SQL queries to filter, aggregate and data cleaning.

Microsoft Excel: For easy-to-use database manipulation, including VLOOKUP and pivot tables

Microsoft Power BI: Used to generate insight through visuals from the dataset as seen in figure 1, 2, 3
and 4, as well as double checking the dataset with tools such as “Column Distribution” and “Column
Profile”.

Dataset Source: Kaggle – Why Do Customers Leave? Can You Spot the Churners? (https://www.kaggle.com/datasets/hassanelfattmi/why-do-customers-leave-can-you-spot-the-churners?select=Status_Analysis.csv)

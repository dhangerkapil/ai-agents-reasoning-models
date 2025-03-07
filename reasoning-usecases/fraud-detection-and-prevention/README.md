# Fraud Detection and Prevention

Banks use advanced fraud detection systems to protect their customers. However, there is a delicate balance between avoiding false positives, which can inconvenience genuine customers, and missing actual fraud cases, which can lead to significant losses. Typically, these systems generate numerous alerts, and Fraud Case Managers must prioritize their efforts on the most probable fraud cases. They use their expertise and combine alerts with other clues and unstructured data to determine if fraud is occurring and then contact the customer.

With the rise in fraud and scams, it is impossible for case managers to address every alert. AI can help banks analyze these alerts and combine structured data from fraud systems with unstructured data sources such as call transcripts and purchase information. This helps prioritize cases for review by Fraud Case Managers, ensuring more customers are protected.

In this scenario, there are 30 potential customer profiles flagged by the fraud system. The task is to prioritize the top 5 most likely fraudulent cases for review by the Fraud Case Manager. The model also aims to predict which of the top 5 are actual fraud cases.

## Files

### transaction-location-analysis.csv
This file contains data about the locations where transactions were made in the last 24 hours and whether any unusual locations were used.

### social-media-activity.csv
This file includes data about the number of positive and negative mentions of customers on social media platforms.

### recent-customer-communications.csv
This file provides data about recent communications between customers and the bank, including the reason for contact and the date of communication.

### merchant-category-code-analysis.csv
This file contains data about the percentage of transactions in different merchant categories for each customer, such as retail, travel, electronics, and gambling.

### internal-audit-flags.csv
This file includes data about internal audit flags for AML (Anti-Money Laundering) and KYC (Know Your Customer) compliance issues for each customer.

### fraud-risk-score.csv
This file contains data about the fraud risk score for each customer, ranging from 0 to 100, indicating the likelihood of fraudulent activity.

### device-usage-patterns.csv
This file provides data about the number of registered devices, new devices used in the last 24 hours, and any suspicious device activity for each customer.

### customer-satisfaction-score.csv
This file includes data about the customer satisfaction score for each customer, indicating their overall satisfaction with the bank's services.

### customer-profiles.csv
This file contains data about the account age, account type, previous fraud history, and VIP status of each customer.

### recent-purchases-customers.csv
This file provides data about recent purchases made by customers, including the item and price.

### transcripts-calls-customers.txt
This file contains transcripts of recent calls between customers and bank agents, detailing various customer service interactions and issues.

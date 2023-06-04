# Finance

For simplicity let us analyse only private credit card transactions, happened in Germany. According to the "DZB" around 1200 such transactions were made on average every second. When a credit card transaction is made, it goes through several stages before the payment is approved or declined. First, the transaction details are sent to a payment gateway where the payment is authorized. The payment gateway then sends the transaction details to a fraud detection system that analyzes the data in real-time to identify any fraudulent activities. The data about transactions may be further analysed by the companies whether internally for decision making or directly for end-customers

## Aim

Minimizing losses from fraudulent activities, financial decision making based on timely insights.

## Mapping

Event - credit card transaction

Producers:
- banks
- credit card companies

Consumers:
- risk managemet systems
- credit score systems (SCHUFA, ...)
- government
- clients (?)

# IoT

17.7 billion worldwide Industrial IoT connections happened in 2020, which will increase to 36B by 2025.

## Aim

Detecting anomalies or events in real-time.

## Mapping:

Event - measurement

Producers:
- sensors
- devices (industrial machinery)

Consumers:
- Analysing center (also producer for further consumers)
- Industrial automation
- Transportation and logistics
- Environmental monitoring (for governmental purposes, like monitoring co2 quotes)



# E-commerce

Amazon.de collects data about 15 Milltions user visits per day. Each visit, lasting 7 Minutes on average, accumulates various user activities, such as such as user clicks, user purchases, and website navigation data. Every action helps forming targeted recommendations in real-time, increasing time a user spending on the platform and helping user to make a product decision. No wonder, that such websites may influence the user's behavior and manipulate prices for increasing the willness to buy. This is only possible due to real-time analysis made by stream processing pipelines

## Aim

Personalized recommendations and targeted advertising in real-time, i.e. understand user-behavior.

## Mapping:

Event - user action

Producers:
- web servers & search engines
- databases
- user devices

Consumers:
- ML systems, such as recommendation or advertising systems.
- Inventory management
- Pricing optimization
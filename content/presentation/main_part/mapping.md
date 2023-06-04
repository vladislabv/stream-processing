# E-commerce

Amazon.de collects data about 15 Milltions user visits per day. Each visit, lasting 7 Minutes on average, accumulates various user activities, such as such as user clicks, user purchases, and website navigation data. Every action helps forming targeted recommendations in real-time, increasing time a user spending on the platform and helping user to make a product decision. No wonder, that such websites may influence the user's behavior and manipulate prices for increasing the willness to buy. This is only possible due to real-time analysis made by stream processing pipelines.

In the context of stream processing, events are typically small units of data that are processed and analyzed in real time as they arrive in a continuous stream. Each event contains information relevant to the specific occurrence or state change it represents.

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

Event - User visits Amazon.de
{"Brower": "Chrome", IP: "82.147.182.19", "session_started": "XXXX-XX-XX XX:XX:XX"}
Consumer - Cache Server, Database
Prducer - User device, e.g. Browser or dedicated application

Real-time analysis: The stream processing system analyzes the incoming events in real time, applying filters, transformations, and aggregations to derive valuable insights.

Auto-complete suggestions: The stream processing system generates auto-complete suggestions for search queries based on the real-time analysis of popular searches and product names.

Product listing: The stream processing system retrieves and processes the relevant product data to generate real-time product listings.

Cart update events: When the user adds items to their cart or modifies quantities, cart update events are generated and published to the stream.

Checkout initiation: The stream processing system handles the user's request to initiate the checkout process, triggering subsequent actions.

Authentication status update: The stream processing system handles the authentication process, updating the user's authentication status in real time.

Shipping address update events: When the user selects or updates their shipping address, the stream processing system generates and publishes shipping address update events.

Delivery option update events: The stream processing system validates and processes the user's selected delivery options, publishing delivery option update events.

Payment method update events: The stream processing system validates the user's selected payment method, generating and publishing payment method update events.

Payment event processing: The stream processing system receives and processes the payment information, performing real-time validation, fraud checks, and generating payment events.

Order update events: Any changes made during the order review trigger the generation and publication of order update events to reflect the modifications.

Order processing: The stream processing system processes the order based on the received events, verifying order data, updating inventory, generating invoices, and triggering fulfillment and shipping processes.

Order confirmation events: Upon successful order processing, the stream processing system publishes order confirmation events to indicate the successful placement of the order.

Payment completion events: The stream processing system processes the payment completion events, verifying the payment status and updating the order data accordingly.

Backend order fulfillment: Backend systems responsible for order fulfillment and shipping subscribe to relevant stream events, retrieve order details, and initiate necessary actions for fulfillment.

Order tracking events: The stream processing system handles requests for order tracking information, retrieving the latest tracking data from the stream and sending it back to the frontend for display.

Delivery confirmation events: Upon receipt of the package, the stream processing system receives the confirmation of receipt, updates the order status, and publishes delivery confirmation events.

## Aim

Personalized recommendations and targeted advertising in real-time, i.e. understand user-behavior.


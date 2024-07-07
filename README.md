# Fraud Delivery Executive Identification using Isolation Forest

This project aims to detect fraudulent delivery executives using the Isolation Forest algorithm. It analyzes data features like undelivered order rates, delivery times, and session data to identify anomalies indicative of fraud. The repository includes data preprocessing, exploratory data analysis (EDA), feature engineering, model implementation with Isolation Forest, and evaluation metrics. This project enhances delivery service integrity by improving fraud detection capabilities.

## Dataset Details

| Field Name            | Description                                                                                      |
|-----------------------|--------------------------------------------------------------------------------------------------|
| order_id              | Unique ID for each order                                                                          |
| order_time            | Time of the creation of order by the client                                                       |
| order_date            | Date of the order                                                                                 |
| allot_time            | Time of allocation of order to the rider                                                           |
| accept_time           | Time of acceptance of the order by the rider (if available)                                        |
| pickup_time           | Time of pickup of the order (if available)                                                         |
| delivered_time        | Time of delivery of the order (if available)                                                       |
| cancelled_time        | Time of cancellation of order (if the order was cancelled)                                         |
| cancelled             | Whether the order was cancelled                                                                   |
| rider_id              | Unique ID for each rider                                                                          |
| first_miledistance    | Road distance from rider’s location to the pickup location                                          |
| last_miledistance     | Road distance from pickup location to the delivery location                                         |
| allotted_orders       | Total number of orders allotted to the rider in the 30 days before (not including) order_date       |
| delivered_orders      | Total number of orders delivered by the rider in the 30 days before (not including) order_date      |
| undelivered_orders    | Total number of orders allotted to but not delivered by the rider in the 30 days before order_date  |
| lifetime_ordercount   | Total number of orders delivered by the rider at any time before order_date                         |
| reassigned_order      | Whether the order was reassigned to this rider                                                     |
| reassignment_method   | If the order was reassigned, whether the reassignment was done manually or automatically            |
| reassignment_reason   | More detailed reason for the reassignment                                                          |
| session_time          | Total time the rider had been online on order_date before order_time                                |

### Dataset Description: Swiggy/Zomato Order Information

The **Swiggy/Zomato Order Information** dataset, created by Bhavik Chandna, is a comprehensive collection of data pertaining to food delivery orders managed by riders. Each order is uniquely identified by an `order_id`, and key timestamps such as `order_time`, `allot_time`, `accept_time`, `pickup_time`, `delivered_time`, and `cancelled_time` provide insights into the order lifecycle. The dataset also tracks whether an order was cancelled (`cancelled`) and if it was reassigned to another rider (`reassigned_order`).

## Key Features
- Data preprocessing and cleaning
- Exploratory data analysis (EDA)
- Feature engineering for anomaly detection
- Isolation Forest model implementation
- Evaluation metrics for model performance
